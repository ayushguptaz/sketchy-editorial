---
name: sketchy-editorial
description: Generate minimalist hand-drawn editorial illustrations for English articles, blog posts, slide decks, documentation, workflows, methodologies, processes, structures, states, metaphors, or arguments. Features a recurring solid-black ink character on pure white backgrounds with sparse red/orange/blue handwritten annotations. Clean, absurd, inventive.
---

# Sketchy Editorial Illustrations

## Core Purpose

Design and generate 16:9 horizontal editorial illustrations for English-language content. The goal is NOT commercial illustration, PPT infographics, or cute cartoons. Instead: turn an article's key judgments, processes, structures, states, or metaphors into a clean, absurd, inventive, readable hand-drawn explanation sketch.

The default visual character is a solid-black ink creature with white dot eyes, thin legs, and a blank expression — seriously doing something absurd but logically sound. This character MUST participate in the core action of the image — never just standing around as decoration.

## Reference Files

Read as needed per task — don't load everything at once:

- `references/style-dna.md`: Style DNA, colors, text rules, prohibitions.
- `references/character-ip.md`: Character IP — appearance, personality, action library, prohibitions.
- `references/composition-patterns.md`: Structure types, original metaphor methods, anti-copying rules.
- `references/prompt-template.md`: Single-image generation prompt template.
- `references/qa-checklist.md`: Post-generation checks and iteration rules.

## Workflow

### 1. Digest the Content

Read the user's article, link, Notion page, Markdown file, or screenshot. Extract:

- What is the core argument or insight?
- Which paragraphs carry a cognitive turning point?
- Which content benefits from visual explanation?
- Which parts are text-only and don't need illustration?

Don't distribute illustrations evenly. Prioritize "cognitive anchors": core judgments, breakpoints, input-output loops, branching logic, before/after contrasts, one-source-many-uses, handoff paths, common pitfalls, role/state changes.

### 2. Produce a Shot List First

If the user asks to "analyze", "plan", or "think about what illustrations to make", provide a shot list. For each illustration specify:

- Placement (after which section/paragraph)
- Theme
- Core meaning
- Structure type
- What the ink character is doing in the image
- Suggested elements
- Suggested English annotation words

Default 4-8 illustrations. Short articles: 1-3. Long articles: never exceed 9. Enough is enough — don't turn prose into a picture book.

### 3. Single-Image Generation

If the user explicitly says "generate", "create", "make the images", don't stop to ask for confirmation — use the built-in `image_gen` tool to generate each image individually. Never combine multiple illustrations into one image.

Each image explains ONE core structure. Every prompt must include:

- 16:9 horizontal editorial illustration
- Pure white background
- Black hand-drawn line art
- Sparse red/orange/blue handwritten English annotations
- Lots of white space
- The ink character as the core action subject
- Prohibit: PPT style, commercial illustration, childish/cute, complex architecture diagrams, type-label titles in the top-left corner

Never replicate past examples. Examples only provide style density and character participation patterns. Every time, invent a new strange-but-valid metaphor from the current content.

### 4. Check and Iterate

After generation, check `references/qa-checklist.md`. If any of these problems appear, regenerate or locally edit:

- Character is just decoration
- Image is too busy
- Looks like a flowchart/PPT
- Too much text or serious typos
- Top-left corner has a type-label title like "Common Pitfalls / Flowchart / System Architecture"
- Style is too cute, childish, or stiff
- Background is not clean white

### 5. Save and Deliver

If the user is working in a workspace, save final images to:

```text
assets/<article-slug>-illustrations/
```

Name sequentially:

```text
01-topic-name.png
02-topic-name.png
```

Preserve original generated files. Don't overwrite existing assets unless the user explicitly asks to replace.

## Output Format

Pre-generation strategy output should be short and precise. Post-generation delivery should include:

- How many images generated
- Each image's purpose
- Save path
- Which images are strongest, which are optional

Don't write long essays about style theory — let the images speak.
