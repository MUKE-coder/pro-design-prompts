# The Human-Made Look: Why People Can Tell It's AI — and How to Stop It

People spot AI images in under a second, and once they do, trust drops. They aren't running a
detector — they're reacting to a handful of **repeatable visual tells**. Remove the tells and the
image reads as "a real photo, designed by a person".

There are two families of tells:
1. **Design tells** — the layout looks like no human made a decision (AI slop).
2. **Photo tells** — the light, skin, textures and physics don't behave like a camera.

The full rules the AI follows are in [AI.md §8](../AI.md). This page explains them.

---

## 1. Design tells (the "nobody decided this" look)

| Tell | Why it gives it away | Fix |
|---|---|---|
| **Frosted-glass panels** (glassmorphism) everywhere | It's the default "modern" finish every generator reaches for | Solid flat fills, real paper/material, or no panel at all |
| **Dark navy + cyan/electric-blue glow** | The statistical average of "tech" | Pick a deliberate 2–3 colour palette with hex; stand out from the feed |
| **Glowing neon outlines** on boxes, logos, pills | Real designers rarely glow everything equally | No glow. Separation from contrast and space |
| **High density** — logo, title, subtitle, list, icons, command, arrow, person | A landing page squeezed into an image | One message. Delete until it breaks, then add one thing back |
| **Feature lists with matching icons** + status labels ("Ready", "Built-in") | Filler: says nothing a human would choose to say | One claim, shown with real proof |
| **Stock icon sets** (shield, padlock-person, gauge, rocket, lightbulb) | The first icon anyone would pick for the word | A real screenshot / product / object — or nothing |
| **Arrows that point at the wrong thing** | Formulaic combinations that don't make sense | Remove, or make it point at the actual payoff |
| **Fake UI, fake code, decorative symbols** (a "+" where a `$` prompt goes) | Looks right at a glance, wrong on inspection | Real screenshots; real, correct commands |
| **Lens sparkle / flare / glints** on logos | Pure AI decoration | Delete |
| **Gradient-filled, glowing headline** | Default "premium" text effect | Flat colour, a named font with character, solid box or stroke if needed |
| **Everything centred and evenly spread** | No hierarchy, no grid | One alignment edge, one dominant element, deliberate asymmetry |

## 2. Photo tells (the "no camera was involved" look)

| Tell | Fix in the prompt |
|---|---|
| **Smooth, waxy, airbrushed skin** | "natural skin with visible pores and texture, no retouching or smoothing" |
| **Coloured rim light** (cyan/blue/purple edge glow) that doesn't match the face | "one light direction; background relit to match the light already on the person; no coloured rim light" |
| **Pasted-in person** — no contact shadow, hard edges, different sharpness | "clean natural hair edges, contact shadows where hands meet the desk/laptop, matching grain and sharpness" |
| **Perfect symmetry** in faces, rooms, shelves | "imperfect, asymmetrical real-world details" |
| **Generic blurred blue "studio" background** with bokeh orbs | A plain colour, a real place, or a real screenshot — lens-like blur only if justified |
| **Over-saturated HDR, everything sharp** | "true-to-life colour, normal saturation, realistic 35mm/50mm depth of field, light natural grain" |
| **Hands, glasses, jewellery, reflections slightly wrong** | "5 fingers, correct joints, natural grip; reflections and glasses physically consistent" |
| **Melted or nonsense background objects, gibberish signs** | Keep the background simple; "no background text" |

## 3. The single biggest fix: use the real photo, and change the scene — not the face

When the user supplies a real camera photo of themselves:
- Use it **exactly**. No beautify, no smoothing, no reshaping, no regenerated face. A real face
  with pores and asymmetry is the strongest "human" signal in the whole image.
- **Read its light** (direction, softness, colour temperature) and make the rest of the image agree.
- If the photo is weak, **reshoot** — a phone at eye level, facing a window, 2–3 expressions — rather
  than asking the AI to "fix" the face.
- When the generator keeps drifting the face, **composite by hand**: generate the background and
  text area, then place the real cut-out in Photoshop / Photopea / Canva / Figma.

## 4. The deletion pass

After every generation, name the **3 things that most say "AI made this"**, remove them, and
replace them with empty space or a real asset. Repeat until nothing jumps out.

> If you can delete it and the message still works, it was slop.

## 5. Copy-paste block

```text
HUMAN-MADE FINISH: This must look like a real photograph taken with a real camera and laid out by a
professional human designer — not an AI image. One consistent light direction across the whole
image; background lighting matched to the light already on the person. Natural skin with visible
pores and texture, no retouching or smoothing. Natural colour, normal saturation, subtle natural
grain, realistic lens depth of field. Flat, solid design elements only — no frosted glass, no glow,
no neon outlines, no gradients on text, no lens flare, no sparkles, no generic icons, no decorative
labels. Only the exact text listed; every word spelled exactly.
```

> **Note on scope:** these rules are about how the image *looks* — design and photographic
> quality. They don't touch file metadata or content-credential labels that some tools attach, and
> they don't change any platform's disclosure rules for AI-generated or altered content. Follow
> those as they apply to you.
