# ChatGPT / GPT Image

**Strengths:** very literal instruction following, strong text rendering, conversational
editing, understands layout language ("top-left", "60% of the width"), can use uploaded
images (your product photo, logo, or a style reference).
**Weaknesses:** a default "polished stock" look if you're vague; tends to add extra
decorative elements; sometimes renders a *mockup* (poster on a wall) when you say "poster".

---

## Prompt format

Full sentences, structured in labelled sections. Long prompts are fine.

```text
Create a flat 2D social media ad design (not a mockup, not a photo of a poster),
edge-to-edge, 4:5 portrait.

BACKGROUND: solid deep blue #0B2A6F with a soft radial lighter-blue glow behind the product.

HERO: an aluminium energy-drink can (generic, unbranded silver and blue), oversized so it is
taller than the canvas, tilted 20° to the right, covered in cold condensation droplets,
cropped by the right and bottom edges. Hard backlight creating a bright rim along the edges.

TEXT (render exactly as written, correct spelling, no other text anywhere):
- Top-left, very large, heavy italic condensed sans-serif, white, all caps, tight leading,
  three lines: "FUEL" / "YOUR" / "DAY"
- Under it, small regular sans-serif, white at 80% opacity: "Boosts energy and keeps you going."
- Under that, a small white pill-shaped button with dark blue text: "Buy Now →"

LAYOUT: 7% margins, all text left-aligned to the same margin, about 35% empty background.
STYLE: premium beverage campaign art direction, high contrast, crisp.
DO NOT INCLUDE: sparkles, lens flare, splash, ice cubes, extra cans, fake logos, extra text,
drop shadows on text, purple tones.
```

## Tips
- **Say "flat graphic design, edge-to-edge, not a mockup"** to avoid the poster-on-a-wall problem.
- **"Render the text exactly as written"** + **"no other text anywhere"**.
- **Upload references**: "Use the uploaded logo exactly; place it top-left at 10% of width."
  / "Use the uploaded product photo exactly as is; do not redraw or alter the product."
- **Edit in the same chat**: "Keep everything the same. Only make the headline 20% bigger."
- **Aspect ratio**: state it (portrait 4:5 / 2:3, landscape 3:2 / 16:9, square). If the tool
  only supports a few sizes, choose the closest and crop.
- **Transparent background** (for stickers/logos): ask for "transparent background PNG" — supported in many OpenAI image tools.
- If it keeps adding junk, add: "Minimalist. Fewer elements is better. Leave the empty areas empty."
