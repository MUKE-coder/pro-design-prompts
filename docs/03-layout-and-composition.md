# Layout & Composition

Spacing, rhythm and alignment shape how a design *feels* more than colour does.
Image models don't know grids — so you describe the grid in plain words and positions.

---

## 1. Formats (set this first — it changes everything)

The AI always asks **what you're making and where you'll post it** before designing. The full
platform table with safe zones is in [AI.md §2](../AI.md).

| Placement | Ratio | Pixels (typical) | Detail level |
|---|---|---|---|
| Instagram / Facebook feed | **4:5** | 1080×1350 | Medium — must read at thumbnail size |
| Instagram square | 1:1 | 1080×1080 | Medium |
| Story / Reel / WhatsApp Status / TikTok | **9:16** | 1080×1920 | Keep top 14% and bottom 20% free of text (UI covers it) |
| YouTube thumbnail | 16:9 | 1280×720 | Very low — ≤ 4 words, bottom-right clear (see [10-thumbnails.md](10-thumbnails.md)) |
| X / LinkedIn landscape | 16:9 | 1600×900 | Low — 3 words max |
| A4 / A3 flyer & poster (print) | **≈ 1:1.414** (use 2:3 or 3:4 if the model lacks it) | 2480×3508 @300dpi | High — can hold details, still one hero |
| Roll-up banner | 1:2.5 (approx) | 850×2000mm | Headline in top third (eye level) |
| Billboard | 3:1 or 4:1 | — | Very low — 7 words max, read in 3 seconds |
| Carousel slide | 4:5 | 1080×1350 | Consistent system across slides |

> Most image models output at fixed sizes. Generate at the correct ratio, then **upscale**
> (Topaz, Magnific, Krea, Upscayl, or the model's own upscaler) for print.

---

## 2. Describe the grid in words

Models respond to **positions, fractions and percentages**, not to "12-column grid".

**Canvas zones vocabulary**
```
┌─────────┬─────────┬─────────┐
│ top-left│top-centre│top-right│   ← "top third"
├─────────┼─────────┼─────────┤
│mid-left │ centre  │mid-right│   ← "middle third"
├─────────┼─────────┼─────────┤
│ bot-left│bot-centre│bot-right│  ← "bottom third"
└─────────┴─────────┴─────────┘
  "left third" "centre"  "right third"
```

**Good phrases**
- "Headline occupies the top-left, spanning about 60% of the width."
- "Product sits in the right half, bottom-aligned, its top reaching 70% of canvas height."
- "Text column on the left 45%; image on the right 55%."
- "Outer margins of 7% on all sides; nothing touches the edge except the product, which bleeds off the right."
- "All text left-aligned to the same vertical margin."

---

## 3. Proven layout archetypes

Pick one per design. Name it in the prompt.

### A. Split (text left / hero right) — product ads, promos
```
┌───────────────┬───────────┐
│ LOGO          │           │
│ HEADLINE      │   HERO    │
│ HEADLINE      │  (bleeds  │
│ subline       │   right)  │
│ [CTA]         │           │
└───────────────┴───────────┘
```
### B. Headline-top / hero-bottom — flyers, food, posters
```
┌───────────────────────────┐
│ small kicker              │
│ BIG HEADLINE              │
│ BIG HEADLINE              │
│        ┌────────┐         │
│        │  HERO  │         │
│ details│        │  [CTA]  │
└────────┴────────┴─────────┘
```
### C. Full-bleed photo + text in the calm area — lifestyle, fashion, events
Text sits over sky/wall/shadow; subject looks *toward* the text.

### D. Typographic poster — events, quotes, announcements
Type IS the image. Huge headline filling 60–80% of canvas; tiny details at bottom.

### E. Centred hero (only for premium/minimal) — luxury, tech
One object, huge empty space, small headline above, tiny CTA below. Centred is fine
*when the space around it is enormous*.

### F. Educational carousel slide — like the reference carousel
```
┌───────────────────────────┐
│ 01.                       │
│ Bold Title Line           │
│ Grey Second Line          │
│ grey intro sentence       │
│ black instruction sentence│
│ ┌─────────┐ ┌─────────┐   │
│ │ BEFORE  │ │  AFTER  │   │
│ └─────────┘ └─────────┘   │
│ (Before) note (After) note│
└───────────────────────────┘
```

---

## 4. Spacing system

- **Proximity ratio 1 : 3** — gap inside a group is ⅓ of the gap between groups.
- **Margins** 6–8% of width. Premium: 10%+.
- **Empty space** 30–50% of the canvas. Loud sale ads can go to ~20%, never 0%.
- **One alignment edge**. Mixed alignment (some centred, some left) looks amateur.
- **Safe zones** for stories: keep text out of the top ~250px and bottom ~350px at 1080×1920.

---

## 5. Camera & framing vocabulary (for the hero)

| You want | Say |
|---|---|
| Power, heroic product | "low angle, looking up, 35mm" |
| Natural, honest | "eye level, 50mm" |
| Flattering portrait, blurred background | "85mm, f/1.8, shallow depth of field" |
| Flat-lay / menu | "top-down overhead shot, 90°" |
| Drama, motion | "Dutch angle tilted 15°", "motion blur on background" |
| Texture, appetite | "macro close-up, 100mm macro" |
| Product cut-out feel | "studio shot on seamless backdrop" |
| Energy | "product cropped by the frame edge", "oversized, bleeding off canvas" |

---

## 6. The eye path test

Ask: *Where does the eye land first, second, third?* Write that order into the prompt:
> "Reading order: (1) the shoe, (2) the headline, (3) the subline, (4) the CTA button."

Tools to steer the eye: **size, contrast, a person's gaze, lines/diagonals, isolation (space around it).**
