---
name: personal-illustration-styles
description: Maintain and apply the user's private illustration style library. Use when analyzing attractive reference images, extracting a reusable drawing style, adding or refining a style card, selecting a saved style, or writing image-generation prompts that should follow one of the user's collected visual styles.
---

# Personal Illustration Styles

Use this skill as an extensible private style library. Keep reusable visual language separate from the subject matter of any single reference image.

## Route the Request

1. For applying or choosing a saved style, read `references/style-index.md`, then read only the selected style card.
2. For extracting a style from new reference images, follow **Add or Update a Style**.
3. For combining styles, name the dominant style and list no more than two borrowed traits from another style. Avoid vague style soup.

## Apply a Saved Style

1. Separate the requested content from the style:
   - Content: topic, message, objects, characters, required text.
   - Style: composition, linework, color, texture, typography, visual grammar.
2. Read the selected style card and preserve its non-negotiable traits.
3. Adapt composition to the requested aspect ratio and information density.
4. Build the generation prompt in this order:
   - Deliverable and subject
   - Composition and reading path
   - Characters and objects
   - Linework, color, texture, and typography
   - Required text and emphasis hierarchy
   - Negative constraints
5. When generating an image, inspect the result against the style card's checklist and revise the prompt if key traits drift.

Do not copy signatures, watermarks, logos, or creator handles from reference images. Do not describe a style only by naming a living artist or creator; describe observable visual traits instead.

## Add or Update a Style

1. Inspect all supplied references together. Distinguish recurring traits from one-image accidents.
2. Extract these dimensions:
   - Overall mood and intended use
   - Canvas, composition, hierarchy, and reading path
   - Shapes, characters, objects, and icon language
   - Linework, texture, shading, and rendering
   - Palette, contrast, and emphasis colors
   - Typography, labels, annotations, and repeated motifs
3. Record both:
   - Non-negotiable traits that make the style recognizable
   - Flexible traits that may change with subject or aspect ratio
4. Create or revise one file under `references/styles/` using `references/style-card-template.md`.
5. Add the style to `references/style-index.md`.
6. Store useful source images under `assets/styles/<style-slug>/references/`. Use descriptive filenames and never treat source text, signatures, or watermarks as style requirements.
7. Include a reusable base prompt, negative constraints, and a short quality checklist.

Prefer expanding an existing style card when new images clearly belong to it. Create a new card when the references introduce a materially different visual grammar.

## Library Rules

- Use lowercase hyphenated English slugs for folders and filenames.
- Keep the index brief; put details in style cards.
- Describe what is visible, not what is merely assumed.
- Preserve meaningful variation instead of averaging every reference into one generic style.
- Treat reference images as inspiration and analysis material, not assets to reproduce verbatim.

