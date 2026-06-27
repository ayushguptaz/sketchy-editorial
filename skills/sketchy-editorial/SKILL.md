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

### 3. Elaborate the Metaphor (MANDATORY before generating)

Before writing any prompt, run this 3-step elaboration for EACH image. This is what makes the prompts rich and specific:

**Step A — Physical action:** Replace the abstract idea with a concrete physical action the character performs. Don't say "self-doubt exists" — say "the character is trying to walk forward but its own shadow grabs its ankle and pulls backward." Be specific about body position, limb action, direction of movement.

**Step B — Low-tech object:** Replace any system/concept with a simple pen-drawable object. Don't say "mental pressure" — say "a stack of boxes piling on top of the character" or "a ruler getting shorter each time it measures itself." Pick from: boxes, circles, lines, arrows, funnels, drawers, pipes, wells, ladders, ropes, pulleys, scales, doors, squiggles, stacks, loops.

**Step C — Scene choreography:** Describe the FULL scene in 4-6 sentences. Include: where the character is positioned, what its stick limbs are doing, what objects surround it, how arrows or lines show movement/flow, what's happening at each side of the image. Be cinematic in description, mundane in vocabulary.

Write the Composition field with ALL of this detail. A good Composition is 4-8 sentences long, not 1-2.

### 4. Single-Image Generation

If the user explicitly says "generate", "create", "make the images", don't stop to ask for confirmation — use the built-in `image_gen` tool to generate each image individually. Never combine multiple illustrations into one image.

Each image explains ONE core structure. Every prompt must include:

- 16:9 horizontal flat 2D pen sketch on blank white paper
- Pure white background, no texture
- Black hand-drawn pen line art — wobbly, imperfect, like a ballpoint doodle
- FLAT 2D ONLY: no 3D, no shading, no depth, no color fills, no lighting, no rendering
- Sparse red/orange/blue used ONLY for short handwritten word labels — never as fills
- Lots of white space (at least 35% blank)
- The solid-black ink blob character as the core action subject
- All objects drawn as simple outlines: boxes, circles, lines, arrows — no realistic objects
- Prohibit: PPT style, commercial illustration, childish/cute, complex architecture, 3D rendering, digital art, colored illustration, material rendering (glass/metal/glow)

When describing compositions, use SKETCH VOCABULARY: box, circle, line, arrow, blob, squiggle, stick, outline. Avoid words that trigger realism: glass, metal, crystal, transparent, glow, spark, shine, stone, marble.

Never replicate past examples. Every time, invent a new strange-but-valid metaphor using only simple pen-drawable shapes.

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

When delivering prompts (because image_gen is unavailable or user wants prompts only):

- Output each prompt as a plain paragraph of text. NO blockquotes (no `>` prefix lines). NO code blocks. Just a plain paragraph under each image heading.
- Keep it short: image title, one-line description of what it shows, then the prompt as a regular paragraph.

When image_gen is available and generation succeeds:

- How many images generated
- Each image's purpose
- Save path
- Which images are strongest, which are optional

Don't write long essays about style theory — let the images speak.
