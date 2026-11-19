# Template: Educational Carousel (like the reference post)

A carousel is a **system**, not 8 separate images. Define the system once, then repeat it
word-for-word in every slide prompt. Generate all slides in **one chat thread**.

## Step 1 — The System block (paste at the start of every slide prompt)
```text
CAROUSEL SYSTEM (identical on every slide):
- Format: 4:5 portrait, 1080×1350, flat 2D graphic design, not a mockup.
- Background: warm off-white #FAF8F5, plain, no texture.
- Margins: 8% left/right, 7% top. All text left-aligned to the same margin.
- Typeface: ONE neo-grotesk sans-serif family (like Inter Display / SF Pro Display).
- Slide number: top-left, small regular black, format "01." 
- Title: two lines, extra-bold, tight tracking, line-height 1.0, ~7% of canvas height per
  line. Line 1 near-black #111111; Line 2 mid-grey #8A8A8A.
- Intro sentence: regular, ~2.4% height, grey #6B6B6B.
- Instruction sentence: regular, ~2.4% height, near-black #111111.
- Content area: lower 55% of the canvas.
- Small pill labels: "Before" in light grey pill with black text; "After" in black pill with
  white text; each followed by a short 2-line grey note.
- Bottom-right: a small dark-grey circular icon. Progress dots centred at the very bottom.
- No other decoration, no gradients, no shadows except a very soft shadow under cards.
```

## Step 2 — Slide plan
| # | Role | Title L1 / L2 |
|---|---|---|
| 1 | Hook / cover | "[Your design isn't boring]" / "[because of AI]" |
| 2–7 | One tip each, before/after | "[Tip]" / "[Tip continued]" |
| 8 | Summary + CTA | icon row recap + "Save this" + "Follow" bar |

## Step 3 — Tip slide prompt
```text
[PASTE CAROUSEL SYSTEM]

THIS SLIDE (number "[03.]"):
Title line 1: "[Make Your Type]"   Title line 2: "[Work Harder]"
Intro: "[Using more fonts won't automatically improve your design.]"
Instruction: "[Choose one strong typeface, explore different weights, adjust letter spacing,
and create intentional text sizes.]"

CONTENT: two rounded-corner cards side by side, equal size, small gap between them.
- LEFT card "Before": [describe the weak version — light grey background, generic small
  title, grey button, product centred, everything same weight].
- RIGHT card "After": [describe the strong version — dark background, huge bold italic
  headline, dramatic product angle with coloured rim light, white pill button].
Under left card: pill "Before" + note "[Generic typography feels plain and forgettable.]"
Under right card: pill "After" + note "[A clear, bold type hierarchy creates impact.]"

Render all text exactly as written; no other text. Use fictional/unbranded products in the
cards unless I upload my own brand assets.
```

## Step 4 — Summary slide prompt
```text
[PASTE CAROUSEL SYSTEM]
THIS SLIDE (final, no number):
Title line 1 (black): "[Good Design Isn't About Adding More.]"
Title line 2 (grey): "[It's about making better decisions.]"
A row of [6] small rounded-square light-grey tiles, each with a simple black line icon and a
tiny label below: "[Hierarchy]" "[Contrast]" "[Typography]" "[Spacing]" "[Variation]" "[Visuals]".
A thin light divider line. Then a bookmark line icon with text "[Save this for your next
design project.]". At the bottom, a full-width black rounded bar: left text in white
"[Follow for more design content]", a thin vertical divider, "[@yourhandle]", and a white
circle with a black arrow on the right.
```

> **Cover slide tip:** the cover is the only slide that breaks the system — make the hook
> headline 2× bigger and use one striking before/after teaser image.
