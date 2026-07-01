# Lifang Illustration Styles

[中文](./README.md) | English

This repository contains a personal illustration style library Skill for Codex and other local agents that support Agent Skills. It helps an agent choose an illustration style from article content and generate more stable prompts that stay close to curated reference images.

Currently it includes one Skill:

```text
skills/personal-illustration-styles/
```

The Skill stores reusable visual styles as style cards. When you find new attractive illustration styles later, you can keep adding them to the same Skill.

## Available Styles

| Style | Best for | Signature traits |
|---|---|---|
| Hand-drawn knowledge comic | Chinese knowledge cards, AI/workplace ideas, process explainers, social posts | Warm beige paper, shaky black lines, colored pencil, stick figures, sticky notes, orange wavy emphasis |
| Colorful AI whiteboard infographic | LLM/RAG/Agent/MCP, AI technical explainers, architecture maps, course-style blog visuals | White background, bold marker title, colorful panels, robot narrator, technical icons, dense whiteboard poster |
| Warm handdrawn card series | Chinese article cards, social knowledge cards, AI/workplace/product explainers | Warm paper, huge handwritten title, orange keyword, page badge, rounded numbered panels, bottom takeaway |
| Warm handdrawn blog illustration | Blog hero images, newsletter/Zhihu/CSDN article visuals, horizontal section illustrations | 16:9 warm paper scene, hand-drawn title, central metaphor, light labels and arrows, no page badge by default |
| Handwritten lecture notes landscape | Horizontal blog/article explainers, workshop-style diagrams, old/new comparisons | 16:9 off-white paper, blue-gray handwritten title, black note text, yellow highlights, boxes and arrows, no format label in corner |
| Handwritten lecture notes portrait | Vertical note pages, long Chinese explainers, step-by-step study sheets | A4-like off-white paper, blue-gray title, black handwriting, yellow highlights, flow boxes, side notes, bottom summary |

## Preview

### Hand-drawn knowledge comic

| Full Knowledge-Comic | Low-Density Simple Variant |
|---|---|
| ![full density hand drawn](./examples/hand-drawn-full-density.png) | ![simple hand drawn test](./examples/hand-drawn-simple-test.png) |

### Colorful AI whiteboard infographic

| AI System Evolution | Codex Guide for Knowledge Workers |
|---|---|
| ![AI system evolution](./examples/colorful-whiteboard-evolution-test.png) | ![Codex guide](./examples/colorful-whiteboard-codex-guide.png) |

| Workflow Library Example | MCP Stage Poster |
|---|---|
| ![Workflow library](./examples/colorful-whiteboard-workflow-library.png) | ![MCP poster](./skills/personal-illustration-styles/assets/styles/colorful-ai-whiteboard-infographic/references/05-mcp-stage-poster.png) |

### Warm handdrawn card series

| AI Career Rules Card |
|---|
| ![Warm handdrawn card series career rules](./examples/warm-handdrawn-card-series-career-rules.png) |

### Handwritten lecture notes

| Landscape Notes | Portrait Notes |
|---|---|
| ![Handwritten lecture notes landscape career rules](./examples/handwritten-lecture-notes-landscape-career-rules.png) | ![Handwritten lecture notes portrait career rules](./examples/handwritten-lecture-notes-portrait-career-rules.png) |

## Installation

### Option 1: Manual Codex Installation

Clone this repository:

```bash
git clone https://github.com/STRUGGLE1999/lifang-illustration-styles.git
```

macOS / Linux:

```bash
mkdir -p ~/.codex/skills
cp -R lifang-illustration-styles/skills/personal-illustration-styles ~/.codex/skills/
```

Windows PowerShell:

```powershell
New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.codex\skills" | Out-Null
Copy-Item -Recurse -Force ".\lifang-illustration-styles\skills\personal-illustration-styles" "$env:USERPROFILE\.codex\skills\personal-illustration-styles"
```

Restart Codex or open a new session, then use:

```text
Use $personal-illustration-styles to read this article, choose a suitable illustration style, and generate an illustration prompt.
```

### Option 2: skills CLI

If your environment supports the skills CLI:

```bash
npx skills add STRUGGLE1999/lifang-illustration-styles
```

If your skills CLI only supports installing a single Skill directory, use the manual installation method instead.

## Usage Examples

```text
Use $personal-illustration-styles to read this article, decide which illustration style fits, and generate an image.
```

```text
Use the hand-drawn knowledge comic style from $personal-illustration-styles to create a full-density illustration for this AI productivity article.
```

```text
Use the colorful AI whiteboard infographic style from $personal-illustration-styles to create an evolution comparison poster for this LLM/RAG/Agent/MCP article.
```

```text
Use the handwritten lecture notes landscape style from $personal-illustration-styles to create a horizontal handwritten note illustration for this workplace article.
```

```text
Use the handwritten lecture notes portrait style from $personal-illustration-styles to create a vertical handwritten note page for this article.
```

## Adding New Styles

1. Prepare several reference images that clearly belong to the same visual direction.
2. Ask Codex to use `$personal-illustration-styles` to analyze the image style.
3. Create or update `skills/personal-illustration-styles/references/styles/<style-slug>.md`.
4. Put reference images under `skills/personal-illustration-styles/assets/styles/<style-slug>/references/`.
5. Update `skills/personal-illustration-styles/references/style-index.md`.
6. Test the style with a real article and calibrate until the output is close to the references.

## Repository Structure

```text
.
├── README.md
├── README.en.md
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

## License

MIT License
