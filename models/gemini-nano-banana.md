# Google Gemini / Nano Banana

**Strengths:** photoreal people and products, excellent conversational editing (keeps the
rest of the image consistent), multi-image input (product + logo + style reference),
character/product consistency across a series, good text rendering in the Pro/2 models.
**Weaknesses:** can drift to a "too perfect" glossy look; may change small details on each
edit unless you lock them.

---

## Prompt format

Describe the scene like a photographer **and** a designer, in natural paragraphs.
Gemini responds well to *why* ("so the headline has a calm area to sit on").

```text
Design a 4:5 Instagram ad for a fast-food chicken burger. This is a flat graphic design
layout, edge-to-edge, not a mockup.

The background is solid deep red (#C8102E). A single oversized golden-yellow curved shape
bleeds off the top-right corner, cropped by the frame, to add energy without clutter.

The hero is a crispy chicken burger with a sesame bun, fresh lettuce and creamy sauce,
shot in a front three-quarter view with warm side light at 45°, real texture, no steam.
It's large, in the lower right, slightly cropped by the bottom edge.

Typography uses one rounded extra-bold sans-serif family. Top-left headline on two lines:
"Chicken" in white and "Burger" in golden yellow (#FFC72C), very large, tight leading.
Below it, small white regular text: "A classic favourite for any time of the day."
No other text.

Keep 7% margins and leave the area around the headline calm and empty.
Exclude: steam, smoke, floating ingredients, extra food items, drop shadows on text.
```

## Editing workflow (Gemini's superpower)

1. Generate the base.
2. Lock & change one thing:
   ```text
   Keep the composition, product, colours, lighting and all text exactly the same.
   Only change: make the burger 15% larger and move it slightly lower.
   ```
3. Repeat — one change per turn.

## Multi-image tips
- "Image 1 is my product — keep it exactly. Image 2 is my logo — place it top-left small.
  Image 3 is a style reference — match its colour palette and lighting, not its subject."
- For a carousel/series, keep everything in **one chat** and say "same design system as the previous slide".

## Aspect ratio
Choose it in the tool's settings when available, and also state it in the prompt.
