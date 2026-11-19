# Midjourney

**Strengths:** the best aesthetic taste — lighting, mood, editorial and cinematic visuals.
Style references (`--sref`) make series consistent.
**Weaknesses:** text is unreliable (independent tests: usable multi-word text only a minority
of the time); loves to add its own "artistic" extras; less literal with exact layout.

**Best use:** generate the **visual** with deliberate empty space → add text elsewhere
(ChatGPT / Gemini / Ideogram edit, or Canva / Figma).

---

## Prompt format

Shorter. Most important thing first. Comma-separated visual phrases. Parameters at the end.

```text
advertising poster layout, oversized aluminium energy drink can tilted diagonally, cold
condensation droplets, cropped by right edge, deep blue background with soft radial glow,
hard backlight rim, large empty space on the left third for a headline, premium beverage
campaign, high contrast, crisp studio photography --ar 4:5 --style raw --stylize 100
--no text, letters, logo, sparkles, lens flare, splash, ice, extra cans, purple
```

## Parameters that matter (check `/settings` and docs for your version)
| Param | Use |
|---|---|
| `--ar 4:5` / `9:16` / `2:3` / `16:9` | aspect ratio — always set it |
| `--style raw` | less Midjourney "beautification", more literal; use for design work |
| `--stylize 0–1000` (`--s`) | lower (50–150) = follows prompt; higher = more artistic liberty |
| `--no a, b, c` | negative prompt — put your ban list here |
| `--sref <url or code>` | style reference — lock a look across a campaign |
| `--cref` / omni-reference (version dependent) | keep a character/object consistent |
| `--chaos 0–100` | variety among the 4 results; keep low (0–15) for controlled briefs |
| `--seed` | reproduce a result for small changes |

## If you must have text in Midjourney
- ≤ 3 short words, in "double quotes": `headline text "RUN FURTHER" in bold condensed white letters`
- Expect re-rolls. Fix in the Editor / Vary Region, or overlay in Canva.

## Tips
- Write **"large empty space on the [left third / top] for text"** — Midjourney respects this well.
- Don't stack adjectives ("beautiful, stunning, amazing") — they push toward slop.
- Use real photography terms: lens, light setup, film stock, angle.
- Moodboards / personalization profiles: build one from your swipe file for a brand look.
