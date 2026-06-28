# Lifang Illustration Styles

中文 | [GitHub 仓库](https://github.com/STRUGGLE1999/lifang-illustration-styles)

这是一个私人插图风格库 Skill，用于让 Codex / 支持 Agent Skills 的本地智能体根据文章内容自动选择插图风格，并生成更稳定、更接近参考图的提示词。

当前包含一个 Skill：

```text
skills/personal-illustration-styles/
```

它会把不同插图风格沉淀成可复用的 style card。以后看到新的好看图片，可以继续把新风格补充进这个 Skill。

## 当前风格

| 风格 | 适合内容 | 特征 |
|---|---|---|
| Hand-drawn knowledge comic | 中文知识卡片、AI/职场观点、流程解释、社媒长图 | 暖米色纸张、抖动黑线、彩铅、火柴人、便利贴、橙色波浪强调 |
| Colorful AI whiteboard infographic | LLM/RAG/Agent/MCP、AI 技术科普、架构图、课程讲义 | 白底、粗马克笔标题、彩色分栏、机器人讲解员、技术图标、高密度白板海报 |

## 效果预览

### Hand-drawn knowledge comic

| 饱满知识漫画版 | 低密度简版 |
|---|---|
| ![full density hand drawn](./skills/personal-illustration-styles/assets/styles/hand-drawn-knowledge-comic/references/05-full-density-calibration.png) | ![workflow hand drawn](./skills/personal-illustration-styles/assets/styles/hand-drawn-knowledge-comic/references/02-conveyor-workflow.png) |

### Colorful AI whiteboard infographic

| AI 系统演进总览 | MCP 阶段讲义 |
|---|---|
| ![AI system evolution](./skills/personal-illustration-styles/assets/styles/colorful-ai-whiteboard-infographic/references/01-ai-system-evolution-comparison.png) | ![MCP poster](./skills/personal-illustration-styles/assets/styles/colorful-ai-whiteboard-infographic/references/05-mcp-stage-poster.png) |

| RAG 阶段讲义 | 上下文工程 |
|---|---|
| ![RAG poster](./skills/personal-illustration-styles/assets/styles/colorful-ai-whiteboard-infographic/references/03-rag-stage-poster.png) | ![Context engineering poster](./skills/personal-illustration-styles/assets/styles/colorful-ai-whiteboard-infographic/references/07-context-engineering-poster.png) |

## 安装

### 方式一：手动安装到 Codex

克隆仓库：

```bash
git clone https://github.com/STRUGGLE1999/lifang-illustration-styles.git
```

macOS / Linux：

```bash
mkdir -p ~/.codex/skills
cp -R lifang-illustration-styles/skills/personal-illustration-styles ~/.codex/skills/
```

Windows PowerShell：

```powershell
New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.codex\skills" | Out-Null
Copy-Item -Recurse -Force ".\lifang-illustration-styles\skills\personal-illustration-styles" "$env:USERPROFILE\.codex\skills\personal-illustration-styles"
```

重启 Codex 或开启新会话后，即可使用：

```text
使用 $personal-illustration-styles，根据这篇文章选择合适插图风格并生成配图提示词。
```

### 方式二：使用 skills CLI（如果你的环境支持）

```bash
npx skills add STRUGGLE1999/lifang-illustration-styles
```

如果你的 skills CLI 只支持单 Skill 目录安装，请改用方式一。

## 使用示例

```text
使用 $personal-illustration-styles，阅读这篇文章，判断适合哪种插图风格，并生成一张配图。
```

```text
使用 $personal-illustration-styles 的 hand-drawn knowledge comic 风格，为这篇 AI 效率文章生成一张饱满知识漫画版插图。
```

```text
使用 $personal-illustration-styles 的 colorful AI whiteboard infographic 风格，为这篇 LLM/RAG/Agent/MCP 技术文章生成演进对比海报。
```

## 如何继续增加新风格

1. 准备几张同一视觉方向的参考图。
2. 让 Codex 使用 `$personal-illustration-styles` 分析图片风格。
3. 新建或更新 `skills/personal-illustration-styles/references/styles/<style-slug>.md`。
4. 把参考图放到 `skills/personal-illustration-styles/assets/styles/<style-slug>/references/`。
5. 更新 `skills/personal-illustration-styles/references/style-index.md`。
6. 用真实文章生成测试图，校准到接近参考图。

## 目录结构

```text
.
├── README.md
├── LICENSE
└── skills/
    └── personal-illustration-styles/
        ├── SKILL.md
        ├── agents/
        │   └── openai.yaml
        ├── references/
        │   ├── style-index.md
        │   ├── style-card-template.md
        │   └── styles/
        └── assets/
            └── styles/
```

## 许可证

MIT License

