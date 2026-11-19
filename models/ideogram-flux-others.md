# Ideogram, FLUX and Others

## Ideogram — the typography specialist
**Strengths:** the most reliable text rendering (multi-line flyers, prices, dates), "Design"
style type, colour palette control, style references, layout-friendly.
**Weaknesses:** can look more "controlled" and less daring than Midjourney.

**Tips**
- Turn **Magic Prompt OFF** (or review it) — it rewrites your prompt with generic adjectives.
- Style type: **Design** for flyers/posters; **Realistic** for photo ads.
- Set the **colour palette** with your hex codes in the palette option.
- Quote all text; put each text block on its own sentence with position and size.
- Use the **negative prompt** field for the ban list.
- Great for: event flyers with date/venue/price, church programmes, menus, price lists.

```text
Event poster design, flat graphic, 2:3 portrait. Deep navy background #0E1A3A with a single
soft warm-gold light beam from the top centre. Typography-led layout using one elegant
high-contrast serif for the headline and a clean light sans-serif for details.
Top: small gold all-caps kicker "SUNDAY 14 DECEMBER 2026". Centre: very large cream serif
headline on two lines "A Night of" / "Worship". Bottom area, small cream sans-serif, three
lines: "Kampala Serena Hotel · 6:00 PM" / "Free Entry" / "Call 0700 000 000".
Generous margins, 45% empty space, no other text.
```
Negative: `extra text, gibberish, clip art, doves, sparkles, lens flare, clutter, drop shadow`

---

## FLUX (Black Forest Labs — FLUX.2, Flux 3, Kontext)
**Strengths:** photorealism, very literal prompt following, good text when quoted, open
weights (local / ComfyUI), Kontext models for editing; newer versions add layout control.
**Weaknesses:** most versions **don't support negative prompts** — "no X" can even *add* X.

**Tips**
- Rewrite exclusions positively: "no clutter" → "only one object on a plain seamless background";
  "no people" → "an empty scene".
- Natural, specific sentences; subject first, then setting, then light, then text, then style.
- Quote text exactly.
- Use **Kontext** to edit: "Change only the headline to '…'; keep everything else identical."

---

## Others (quick notes)
- **Recraft** — great for vector-style graphics, icons, brand-consistent illustrations; exports SVG.
- **Adobe Firefly** — commercially safe training data; integrates with Photoshop (Generative Fill) and Express.
- **Leonardo** — many fine-tuned models, good for game/illustration styles; use its negative prompt field.
- **Seedream / Grok Imagine / Reve** — capable all-rounders; use the general GPT-Image-style prompt.
- **Canva Magic / Dream Lab** — handy, but finish the type in Canva's real text tools, not in the image.

For any model not listed: use the full structured prompt from `SYSTEM_PROMPT.md`; if it has a
negative prompt field, paste the ban list there; if not, phrase exclusions positively.
