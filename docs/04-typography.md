# Typography for Image Models

Image models can't load font files — but they know font *styles* extremely well.
Describe the font by **category + weight + width + case + tracking**, and optionally name a
well-known typeface as a reference ("similar to Helvetica Neue Bold").

---

## 1. One family, many weights

Hierarchy comes from **weight, size, case, width and tracking** — not from adding fonts.

| Level | Size (of canvas height) | Weight | Case | Tracking | Leading |
|---|---|---|---|---|---|
| Headline | 8–20% | Black / Extra-bold | Title or ALL CAPS | Tight (−2 to −4%) | 0.9–1.0 |
| Offer / number | 6–15% | Black | — | Tight | 1.0 |
| Subline | 2.5–4% | Regular / Medium | Sentence case | Normal | 1.3 |
| CTA | 2–3% | Semibold | Title case | Slightly wide | — |
| Details / legal | 1.5–2% | Regular | Sentence case | Normal / +2% | 1.3 |

> Rule of thumb: **headline ≥ 3× subline**. If they look similar, hierarchy has failed.

---

## 2. Font style vocabulary (what to type in the prompt)

| Feeling | Describe as | Reference names models know |
|---|---|---|
| Clean, Swiss, corporate-premium | neo-grotesk sans-serif | Helvetica Neue, Inter Display, SF Pro Display |
| Sporty, fast, aggressive | heavy condensed italic grotesk, all caps | Nike Futura Condensed style, Druk, Tungsten |
| Friendly, food, family | rounded bold sans-serif | Nunito, SF Rounded, Gilroy |
| Geometric, modern, tech | geometric sans | Futura, Montserrat, Poppins |
| Editorial, luxury, fashion | high-contrast didone serif | Didot, Bodoni, Playfair Display |
| Warm, literary, trust | humanist serif | Garamond, Lora |
| Loud, poster, street | ultra-condensed display sans, all caps | Bebas Neue, Anton, Impact-style |
| Retro / 70s | soft chunky serif | Cooper Black style |
| Spiritual / elegant event | refined serif headline + thin sans details | Cormorant + light sans |

**Example**
```text
Typeface: a heavy condensed sans-serif similar to Bebas Neue, all caps, tight tracking.
Same family for all text; subline in the regular weight.
```

---

## 3. Typographic moves pros use

- **Two-tone headline** — split by colour: "Chicken" white / "Burger" yellow.
- **Weight contrast** — "**Timeless** *Style*": bold + italic of the same family.
- **Stacked headline** — one word per line, flush left, tight leading.
- **Grey second line** — line 1 black, line 2 mid-grey (like the reference carousel titles).
- **Number as hero** — "70%" huge, "Up to" small above it, "OFF" medium beside it.
- **Kicker** — tiny all-caps label above the headline ("LIMITED EDITION", "SUNDAY 14 DEC").
- **Text interacting with image** — product overlapping the bottom of the headline letters
  (say: "the product slightly overlaps the lower part of the headline letters, in front of them").

---

## 4. Making text render correctly

1. **Quote every word**: `the headline reads "FUEL YOUR DAY"`.
2. **Say what NOT to write**: `No other text anywhere in the image.`
3. **Keep it short**: headline ≤ 6 words, total ≤ 25 words. Long text = typos.
4. **Spell tricky words in caps or with spacing** if they keep failing: `"KAMPALA" (K-A-M-P-A-L-A)`.
5. **Numbers**: write exactly — `"UGX 50,000"`, `"14.12.2026"`, `"0772 123 456"`.
6. **One text block per line in the prompt** with its position and size.
7. **Check letter by letter** afterwards. Errors look fine at a glance.
8. **Fix text alone**: on editing models, "Keep everything identical, only change the text
   '…' to '…'". If it keeps failing → generate with empty space and add text in Canva/Figma.

> **Hybrid workflow (most reliable for heavy-text flyers):** generate the visual with the
> layout's text areas left EMPTY, then set the real text in Canva/Figma/Photoshop using
> the type specs from your Design Decisions. Pros do this.
