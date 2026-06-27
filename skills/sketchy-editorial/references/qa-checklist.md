# QA Checklist

## Must-Pass Criteria

- Is 16:9 horizontal.
- Looks like a flat 2D pen sketch on white paper — NOT digital art, NOT 3D, NOT colored illustration.
- Background is pure clean white with zero texture.
- Image is overwhelmingly black line art (90%+) with tiny color accents as handwritten words only.
- No color fills, no shading, no depth, no lighting anywhere.
- Ink blob character is present.
- Character performs the core action, not just decoration.
- Invents a new metaphor for the current content — no recycled compositions.
- Image feels absurd, inventive, interesting.
- Clean and airy — main subject doesn't exceed ~60% of canvas.
- One image explains one core structure only.
- English labels are sparse, short, readable.
- Orange used only for main paths or arrows (thin pen lines).
- Red used only for key points, problems, warnings, or results (handwritten words).
- Blue used only for supplementary notes, feedback, or system state (handwritten words).

## Failure Signals (REJECT immediately)

If any of these appear, regenerate — do NOT try to locally edit:

- Image looks 3D, rendered, shaded, or has any depth/lighting.
- Large colored areas, color fills, or painted sections exist.
- Objects look realistic (glass, metal, stone, translucent materials).
- Image looks like digital art, vector illustration, or polished design.
- Top-left has a type-label title like "Common Pitfalls / Workflow / System Architecture / Roadmap".
- Character looks like a mascot, emoji, or cute cartoon.
- Image looks like PPT, courseware, or a formal flowchart.
- Too many elements, too many arrows, too many nodes.
- Text turns into large explanatory paragraphs.
- Background has paper texture, shadow, gradient, cream, or noise.
- Realistic UI screenshots or tech-feel interface.
- Serious typos or unreadable labels.
- Image is too stiff with no absurd metaphor.

## Iteration Methods

- Too generic: Make the character the action subject, add one strange-but-valid metaphor.
- Too complex: Remove nodes, keep only one action and 3-5 short labels.
- Too cute: Emphasize deadpan, blank serious expression, not cute, not mascot.
- Too PPT: Remove titles, borders, neat grids, and excess arrows — switch to hand-drawn scene.
- Text errors: Prefer local edit; if too many mistakes, regenerate with fewer labels.

## Delivery Judgment

A high-quality image should make the reader first think "that's a bit weird", then understand the structure within 1 second.

If the first impression is "tutorial page" rather than "absurd product sketch on white paper", it doesn't pass.
