# Image Generation Prompt Template

Generate each image individually. Replace variables based on article content. Never combine multiple illustrations into one image.

CRITICAL: The output must look like a quick pen doodle on blank white paper. NOT digital art. NOT 3D. NOT colored illustration. Think: whiteboard sketch, napkin drawing, notebook margin doodle.

When writing the Composition field, use SKETCH VOCABULARY only:
- YES: box, circle, line, arrow, stick figure, blob, squiggle, simple outline shape
- NO: glass, metal, crystal, glow, spark, shine, transparent, realistic material words

```text
Generate one standalone 16:9 horizontal hand-drawn pen sketch on blank white paper.

Style (CRITICAL — must match exactly):
This is a simple black pen doodle on white paper. Flat 2D line drawing. Wobbly hand-drawn pen lines. NOT digital art, NOT 3D, NOT rendered, NOT colored illustration, NOT realistic. Think: whiteboard marker sketch or ballpoint pen doodle in a notebook. Pure white background with no texture. Mostly black ink with tiny sparse red/orange/blue handwritten word annotations only. No color fills anywhere. No shading. No depth. No lighting. No gradients.

Recurring character (required in every image):
A small solid-black ink blob creature with two white dot eyes and thin stick legs. Drawn as a simple filled-black irregular shape, like a quick pen scribble filled in. Blank deadpan expression. Must be performing the core action in the scene, not standing aside. Serious and slightly absurd, never cute or mascot-like.

Theme:
{illustration theme from article}

Structure type:
{one of: Workflow / System Fragment / Before-After Contrast / Role-State / Concept Metaphor / Method Layers / Map-Route / Mini Comic Panels}

Core idea:
{the single core meaning this image must convey}

Composition (MUST be 4-8 detailed sentences):
{Describe the full scene in 4-8 sentences using SKETCH VOCABULARY. Include: (1) where the ink blob character is positioned on the canvas, (2) what specific action its stick limbs are performing, (3) what simple pen-drawn objects surround it — boxes, circles, lines, arrows, funnels, ropes, stacks, loops, (4) how arrows or lines show movement or flow, (5) what is happening on the left vs right side of the image, (6) one absurd-but-logical detail that makes the scene memorable. NO realistic objects — only simple pen-drawn shapes. Be specific and cinematic in description.}

Suggested elements:
{element 1} / {element 2} / {element 3} / {element 4}
(Keep elements simple and drawable with a pen: boxes, circles, arrows, lines, squiggles, simple outlines)

English handwritten labels:
{label 1} / {label 2} / {label 3} / {label 4} / {optional label 5}

Color use:
95% black pen lines. The ink blob character is solid black. Tiny bits of red/orange/blue used ONLY for short handwritten word labels (2-4 words each), never as fills or large colored areas. Orange thin arrows for flow direction. Red words for warnings. Blue words for notes.

Constraints:
Flat 2D pen sketch only — absolutely no 3D, no rendering, no shading, no color fills, no realistic objects, no digital art look. One image explains only one core structure. Keep the main subject around 40%-60% of the canvas. Preserve at least 35% blank white space. Use at most 5-8 short handwritten English labels. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not make it a formal diagram, course slide, or dense explainer. Invent a fresh visual metaphor for this specific content. It should look like someone grabbed a pen and sketched this in 30 seconds on white paper.
```

## Image Editing Prompts

Remove a top-left title:

```text
Edit the provided image. Remove only the handwritten title "{text to remove}" and its underline from the top-left corner. Fill that area with the same clean white background, matching the surrounding blank paper. Preserve everything else exactly: characters, labels, paths, line style, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

Enhance absurdity:

```text
Regenerate this illustration with the same core meaning and simple layout, but make the ink blob character more central to the conceptual action. The character should be doing the strange work that explains the idea, not standing beside the diagram. Keep it as a flat 2D pen sketch — clean, sparse, hand-drawn, not cute, not 3D, not rendered.
```
