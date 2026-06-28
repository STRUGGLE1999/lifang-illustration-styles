# Hand-Drawn Knowledge Comic

## Identity

- **Slug:** `hand-drawn-knowledge-comic`
- **Chinese name:** 手绘知识卡片 × 商业观点漫画
- **Best for:** 中文知识卡片、AI 与职场观点、流程解释、左右对比、社交媒体长图、文章配图
- **Mood:** 温暖、亲切、轻松幽默、逻辑清楚，像知识博主在纸上边讲边画
- **Reference assets:** `assets/styles/hand-drawn-knowledge-comic/references/`

## Calibration From Failed Generations

The style must not collapse into a clean presentation slide. Previous failed outputs looked too much like slide diagrams: large empty rounded rectangles, uniform computer-like Chinese font, thick smooth borders, sparse stick figures, straight orange divider lines, flat pastel cards, and little narrative charm.

Correct this by forcing these style anchors in every prompt:

- Use a real paper-note composition, not a slide template.
- Add one visible narrative scene with expressive stick figures doing something, not just standing below boxes.
- Replace large generic boxes with smaller hand-drawn labels, sticky notes, taped notes, UI scraps, thought bubbles, checklists, arrows, and side annotations.
- Keep borders thin, uneven, and pencil-like; avoid thick smooth vector outlines.
- Use orange as selective emphasis: wavy underlines, arrows, check marks, circled words. Do not use long straight orange divider rules as the main design element.
- Make the image feel manually drawn: off-axis boxes, slight wobble, hatch shading, pencil fill, imperfect spacing, small doodle marks.
- For AI characters, prefer a round-head stick-figure coworker labeled "AI" over a cute robot mascot. Robot mascots make the output feel like generic tech illustration.

## Non-Negotiable Traits

- Warm ivory or pale cream paper background with subtle fibers, grain, and a lightly aged notebook feel.
- Black or charcoal pencil/fineliner linework. Lines are thin-to-medium, hand-wobbled, and slightly uneven.
- Round-head stick figures with expressive faces and exaggerated gestures. Their emotion must explain the idea before the viewer reads every label.
- Dense but readable knowledge-comic layout: top hand-written title, middle illustrated explanation, bottom punchline or summary sentence.
- Low-saturation colored pencil fill. Color stays translucent enough that paper texture remains visible.
- Clay orange / orange-red is the only strong accent and is used sparingly for arrows, wavy underlines, key words, ticks, and small callouts.
- Information is broken into many small hand-drawn pieces instead of a few giant presentation cards.
- The final image must look like a scanned hand-drawn explainer, not a vector infographic, not a PowerPoint slide, not a clean UI mockup.

## Flexible Traits

- Structure may be left-right comparison, conveyor/process flow, central-radiation overload, or problem-to-shift-to-result.
- Aspect ratio may be wide landscape for workflows and comparisons, or square for central-radiation single ideas.
- Supporting colors may vary among sage green, pale blue, pale pink, soft yellow, and beige.
- Text density has two approved variants: **full knowledge-comic default** and **low-density simple variant**. Each label should remain short in both variants.

## Density Variants

When the user provides only an article, choose the density automatically from the article content. Use **full knowledge-comic default** unless the article section is visually simple enough for the low-density variant.

## Article Density Decision

When turning an article into an illustration, first extract the section's visual load:

1. Core claim: What is the one sentence this illustration must explain?
2. Structure: Is the idea a process, comparison, cause-effect chain, list of principles, role split, or single metaphor?
3. Visual anchors: Which people, tools, objects, emotions, conflicts, numbers, or repeated motifs can be drawn?
4. Text budget: What 3-10 short labels are actually worth showing?

Choose **full knowledge-comic default** when the article has any of these:

- A process, timeline, workflow, or multi-step method.
- A comparison between old/new, wrong/right, human/AI, before/after, or two roles.
- Three or more meaningful subpoints, examples, constraints, or decisions.
- Multiple actors such as leader, team, AI, customer, reviewer, user, or system.
- A strong article argument that benefits from side notes, warnings, checklists, or quote-like bubbles.
- Social-post or article-card usage where visual richness helps the idea feel worth saving.

Choose **low-density simple variant** when most of these are true:

- The article section contains one simple idea, metaphor, quote, or reminder.
- The illustration is a header, cover, section break, or calm visual accent rather than the main explanation.
- There are fewer than three useful labels after summarizing.
- Extra notes would repeat the same point rather than add meaning.
- The user asks for a cleaner, calmer, more minimal, or less crowded image.

If unsure, choose **full knowledge-comic default** and keep the center logic clear. It is easier to remove notes later than to recover the original rich knowledge-card feeling from an overly sparse image.

### Full Knowledge-Comic Default

This is the preferred default. It should feel closer to a rich social-media knowledge card than a slide.

- Fill roughly 70-85% of the canvas with readable hand-drawn content while preserving margins.
- Include one dominant narrative structure plus many small supporting notes.
- Use 3 main stage labels or role labels, 6-10 sticky notes or mini labels, 2-4 speech/thought bubbles, 1-2 checklist blocks, and several dotted paths, `@` marks, arrows, sparkles, sweat drops, or tiny icons.
- Let the composition feel lively around the edges: corner callouts, taped notes, small reminder bubbles, side checklists, mini progress bars, or tiny audience figures are welcome.
- Keep the center logic clear. The image can be busy, but the reading path must still be obvious.

### Low-Density Simple Variant

Use this variant for sparse concepts, header images, section breaks, or when the user asks for a calmer look.

- Fill roughly 45-60% of the canvas.
- Keep one clear narrative scene with 3-5 supporting labels.
- Use fewer bubbles and side notes, but keep the paper texture, hand-drawn linework, expressive stick figures, sticky notes, orange wavy emphasis, and bottom punchline.
- Do not simplify into a slide: even the simple variant must still feel hand-drawn and story-like.

## Visual System

### Composition

- Use a large loose handwritten Chinese title near the top. The title is black with one orange wavy underline under the key phrase, not a perfectly straight underline.
- Build the middle as a miniature story: characters carry files, point, inspect, shout through a megaphone, sit tired at a desk, push work along a belt, or react to results.
- Use arrows, dotted paths, `@` symbols, sparkles, sweat drops, tiny notes, tape strips, and thought bubbles to guide reading.
- Put the bottom takeaway in black handwritten text, with only one or two key words in orange and wavy-underlined.
- Maintain generous margins and breathing room, but fill the center with lively micro-scenes rather than large empty blocks.
- For article illustrations, default to the full knowledge-comic variant: one clear scene plus rich side callouts, checklists, bubbles, and taped notes. Use 3-5 small callouts only for the low-density simple variant.

### Forms and Characters

- Characters are simple round heads with line bodies, small hands, and oversized expressions.
- Faces use a few marks only: angled brows, dots or curved eyes, open mouth, sweat drop, star eyes, or tired mouth.
- Props are simplified but recognizable: laptop, clipboard, megaphone, file pile, checklist, calculator, AI chat window, magnifier, button, conveyor belt, coffee cup.
- AI roles should usually look like the same stick-figure coworker system as humans: round head, simple body, small "AI" label, headset, laptop, or `@` motion marks. Avoid making AI the only polished mascot in the scene.
- UI windows and panels may appear, but they must be drawn like doodled paper scraps: uneven corners, slight tilt, thin outline, soft colored pencil fill.
- Avoid realistic human anatomy, polished mascot characters, clean corporate illustrations, and perfectly aligned icon systems.

### Linework and Texture

- Use sketchy black linework with slight jitter and pressure variation.
- Use pencil hatching for shadows under characters, behind cards, inside buttons, and under props.
- Fills are hand-colored pencil patches, not flat digital rectangles.
- Keep shadows light and scribbled. Avoid heavy drop shadows, glossy gradients, and 3D depth.
- Leave small imperfections: tilted labels, uneven spacing, hand-drawn arrows, rough circles.

### Palette and Emphasis

- Background: warm white, cream, pale aged paper.
- Main text and outlines: charcoal black or deep gray.
- Strong accent: clay orange, terracotta, orange-red.
- Soft blocks: pale yellow, sage green, dusty blue, pale peach, muted pink.
- The whole image should be low contrast and warm. Avoid saturated neon colors, pure white canvas, and dark backgrounds.

### Typography and Annotations

- All visible text should look handwritten with natural size variation. Do not use clean printed sans-serif or slide-deck typography.
- Title should feel drawn with a thick marker or soft brush pen; small labels should feel like pen handwriting.
- Use short Chinese labels. Prefer 2-8 Chinese characters per label when possible.
- Use handwritten marks: check marks, circles, short arrows, `Zzz`, `7x24`, `@`, star sparkles, tiny locks, small warning marks.
- If the image model cannot render exact Chinese reliably, ask for fewer Chinese phrases and leave some labels as short strokes or blank note areas for later lettering.

## Repeated Motifs

- Sticky notes with tape
- Orange wavy underlines
- Hand-drawn arrows and dotted motion paths
- Thought bubbles and speech bubbles
- Sweat drops, sparkles, star eyes, sleepy `Zzz`
- Checklists, short labels, small badges
- Conveyor belts, file piles, chat windows, magnifiers, laptops

## Common Drift To Avoid

- Clean slide layout with three giant colored cards
- Big smooth rounded rectangles as the main structure
- Cute robot mascot as the main AI figure when a stick-figure AI coworker would match better
- Straight orange horizontal rules at top and bottom
- Uniform printed font
- Overly sparse diagrams with only boxes and arrows
- Thick vector outlines and perfectly symmetrical shapes
- Flat digital pastel fills without pencil texture
- Tiny emotionless stick figures placed as decoration
- Generic corporate infographic, dashboard, whiteboard, or UI mockup style
- Copying reference text, signatures, watermarks, handles, or exact layouts

## Base Prompt

```text
创作一张中文手绘知识漫画信息图，主题为【主题】，核心观点是【观点】。默认使用“饱满知识漫画版”：画面信息要丰富、饱满但不乱，像知识博主手绘长图，而不是PPT、矢量信息图或干净UI图。

构图采用【左右对比 / 流水线流程 / 中心辐射 / 问题—转变—结果】。顶部放一个松弛的黑色手写大标题，只用橙红色波浪线强调关键词。中部画一个有叙事动作的知识漫画场景：圆头火柴人正在【动作：指挥、搬文件、检查、敲按钮、和AI协作等】，周围穿插小便利贴、胶带纸条、标签框、聊天窗口、检查清单、思想气泡、短箭头和虚线轨迹。底部放一句手写金句总结，只把1-2个重点词写成橙红色并加波浪下划线。

饱满度要求：主体逻辑清晰，但四周要有辅助注释和小场景。加入约3个主阶段标签、6-10张小便利贴/短标签、2-4个气泡、1-2个检查清单或小进度条、若干虚线轨迹、@符号、星星、汗滴、勾选和小箭头。信息块要小而多，围绕主流程排布，不要只画三个大框。

视觉风格：暖米黄色旧纸背景，细腻纸纹和轻微颗粒；黑色铅笔/针管笔线稿，线条自然抖动、粗细不完全一致；低饱和彩铅轻涂，能看到纸张质感；阴影用稀疏排线和铅笔涂抹。主色是黑色和暖纸色，强调色是陶土橙/橙红色，辅助色只用浅黄、鼠尾草绿、浅蓝、淡粉。信息块必须小而多、略微倾斜、像手画贴纸，不要使用大块机械圆角矩形。

人物是简单圆头火柴人，表情夸张清楚：眉毛、嘴型、汗滴、星星眼、困惑或得意动作要明显。文字尽量短，像中文手写标注，不要电脑字体。
```

## Low-Density Prompt Add-On

Append this only when choosing the simple variant:

```text
使用“低密度简版”：减少外围注释，只保留一个清楚主场景、3-5个短标签、少量箭头和一个底部金句。画面更清爽，但仍必须像纸上手绘知识漫画，不能变成PPT卡片或简洁矢量图。
```

## Article Illustration Prompt Pattern

Use this pattern when turning an article section into one illustration:

```text
Use case: infographic-diagram
Asset type: Chinese article illustration
Primary request: 为文章段落【段落主题】画一张手绘知识漫画配图，解释【核心观点】。
Density decision: 根据文章内容自动选择【饱满知识漫画版 / 低密度简版】。选择理由：【一句话说明：流程多、角色多、要点多，所以饱满；或单观点、标签少，所以简版】。
Composition: 【选择一个结构】。必须有一个中心叙事场景，不要只画三张卡片。
Required short text: 标题「【短标题】」；标签「【标签1】」「【标签2】」「【标签3】」；底部金句「【短金句】」。
Density: 如果选择饱满知识漫画版，加入丰富但可读的边缘注释、小便利贴、气泡、清单和虚线路径；如果选择低密度简版，保留清楚主场景、3-5个短标签和一个底部金句。
Style: hand-drawn knowledge comic on warm cream paper, shaky black pen, colored pencil, expressive round-head stick figures, sticky notes, tape, arrows, thought bubbles, checklists, dotted paths, small side callouts, orange wavy underline.
Avoid: clean PowerPoint slide, three big rounded cards, printed font, straight orange divider lines, smooth vector graphics, flat UI diagram, exact copied reference layout, watermark.
```

## Negative Constraints

```text
不要照片写实、不要3D、不要光滑矢量插画、不要PPT版式、不要大面积圆角卡片、不要粗黑机械边框、不要均匀电脑字体、不要上下直线橙色分隔线、不要空洞留白、不要纯白背景、不要霓虹高饱和配色、不要复杂写实人物、不要厚重阴影、不要复制参考图中的署名水印或平台标识。
```

## Quality Checklist

- [ ] 看起来像纸上手绘扫描图，而不是PPT或矢量信息图。
- [ ] 顶部标题、中部漫画图解、底部金句三层明确。
- [ ] 中部至少有一个正在行动或强烈反应的圆头火柴人。
- [ ] 有便利贴、胶带、箭头、气泡、短标签等手绘知识图锚点。
- [ ] 默认饱满版有足够边缘注释、气泡、清单和小标签；不是只在中间摆一条流程。
- [ ] 低密度简版仍保留叙事动作和手绘知识图锚点；不是简化成PPT。
- [ ] 只给文章时，已根据文章的流程、角色、要点数量和用途选择密度，而不是机械套默认值。
- [ ] 没有用三张大圆角卡片撑完整个画面。
- [ ] 线条有手抖和铅笔质感，填色有彩铅纹理。
- [ ] 橙红色只用于重点词、箭头、勾选、波浪线，没有变成长直线装饰。
- [ ] 文字像手写短标注，不像正式幻灯片字体。
- [ ] 画面有叙事和情绪，不只是抽象框图。
- [ ] 未复制参考图片的具体文案、署名、水印或品牌标识。

## Reference Notes

- Initial references include landscape process diagrams, a landscape before-after comparison, and a square central-radiation overload composition.
- The stable style grammar is: warm paper + black hand-drawn linework + restrained orange emphasis + expressive stick-figure knowledge comic.
- Failed test images drifted toward sparse slide diagrams. Future prompts must explicitly require lively paper-note comic scenes and forbid giant rounded-card layouts.
- Later calibration confirmed two useful density modes: the rich/full version is the default for article illustrations and social posts; the low-density version is acceptable for simpler content but should not become the default.
- User preference update: when only an article is provided, the skill should decide between full and low-density modes automatically from the article's visual load.
