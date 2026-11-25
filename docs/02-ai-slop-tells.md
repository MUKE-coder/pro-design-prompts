# AI Slop: The Tells and How to Kill Them

"AI slop" is not "made with AI". It's output that shows **no decisions were made** — the model
filled every gap with its statistical average. The fix is always the same:
**replace a generality with a decision.**

A short ban list at the top of a prompt does more than paragraphs of positive description,
because models never avoid their defaults unless told to.

---

## Why image models produce slop

| Cause | What happens | Fix |
|---|---|---|
| Vague adjectives ("modern, clean, stunning") | Model averages every "modern" image it has seen | Name a specific reference + specific decisions |
| Empty space in the brief | Generators *fill* empty space with props, sparkles, steam, text | Say explicitly what goes in the empty space: "nothing — plain background" |
| No hero named | Everything gets equal weight | Name ONE dominant element + its size |
| Unquoted text | Model paraphrases / invents words | Quote every word, say "no other text" |
| One prompt, first result, posted | No editing pass | Generate in rounds; edit by removing |
| Asking for "a poster" | You get a *photo of a poster on a wall* (a mockup) | "flat 2D graphic design file, edge-to-edge, not a mockup" |

---

## The ban list (copy into any prompt)

### Visual tells
- Purple → blue / indigo / pink neon gradients, "cyberpunk" glow
- Lens flares, light leaks, god rays, bokeh orbs, floating particles, sparkles, glitter
- Steam / smoke / mist on everything (especially food)
- Glossy plastic 3D render look, chrome blobs, random abstract 3D shapes
- Over-saturated HDR; everything sharp front to back
- Orange-and-teal colour grade on everything
- Symmetrical, centred, "everything in the middle" composition
- Random decorative swooshes, waves, dots, confetti that mean nothing
- Busy textured backgrounds behind text

- Frosted-glass / glassmorphism cards, pills and tiles; glowing neon outlines around boxes
- Dark navy + electric-blue/cyan "tech" palette with blurry blue studio bokeh
- Feature lists with matching stock icons and filler status labels ("Ready", "Built-in")
- Arrows pointing at the wrong thing; fake UI, fake code, decorative symbols in commands
- Lens sparkle / glint on logos

### People tells
- Waxy / airbrushed / plastic skin, perfect symmetrical faces, dead eyes
- Coloured rim light (cyan/purple edge glow) that doesn't match the light on the face; pasted-in look
- Extra or fused fingers, warped hands, melted jewellery
- Everyone smiling at the camera with identical teeth
- Generic stock poses: pointing at laptop, handshake, thumbs-up, arms crossed in a suit

### Typography tells
- Gibberish or misspelled text; fake brand names; fake URLs; lorem ipsum
- Text the brief didn't ask for (background signs, labels, watermark-like marks)
- More than 2 typefaces; mixed random fonts
- 3D / bevelled / chrome / outlined text, drop shadows and outer glows on text
- Script fonts for anything longer than 2 words
- Headline and body nearly the same size
- Text over busy parts of the image

### Concept tells
- Lightbulb = idea, rocket = growth, globe with network lines = global, brain with circuits = AI
- Copy like "Elevate your experience", "Unlock your potential", "Transform your workflow"
- A design a competitor could post unchanged

> Full photo + design rules for a result that never reads as AI: [09-human-made-look.md](09-human-made-look.md).

---

## Negative-prompt strings (ready to paste)

**General design**
```text
no purple gradient, no neon glow, no lens flare, no sparkles, no particles, no bokeh,
no smoke, no steam, no extra objects, no clutter, no drop shadow on text, no 3D text,
no bevel, no outline text, no watermark, no fake logo, no gibberish text, no extra text,
no mockup, no frame, no border, no wall, no hands holding the poster, no frosted glass,
no glassmorphism, no neon outline, no generic icons, no decorative labels, no gradient text
```

**People**
```text
no plastic skin, no airbrushed skin, no extra fingers, no deformed hands,
no uncanny face, no symmetrical face, no dead eyes, no stock-photo pose,
no retouching, no skin smoothing, no coloured rim light, no face changes
```

**Food**
```text
no steam, no smoke, no excessive garnish, no floating ingredients, no splash,
no glossy plastic look, no oversaturated colours, no dark moody restaurant background
```

**Midjourney format**
```text
--no gradient glow, lens flare, sparkles, particles, extra text, watermark, frame, mockup
```

> **Flux tip:** most Flux versions ignore negative prompts. Rewrite each "no X" as a positive
> instruction: "no clutter" → "a single object on a plain seamless background".

---

## The deletion pass (the most powerful fix)

After the first generation:
1. Name the **3 things** that most scream "AI made this".
2. Remove them. Replace with **empty space**, not with something else.
3. Regenerate or edit. Repeat until the design holds up without them.

> Anything you can delete without missing it was slop to begin with.

**Edit instruction template**
```text
Keep everything exactly the same — layout, text, colours, product — except:
remove [the sparkles around the product], remove [the glow behind the headline],
and replace [the patterned background] with a plain solid [#hex] background.
```
