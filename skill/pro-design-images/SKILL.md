---
name: pro-design-images
description: Use before generating or prompting any image model to make a YouTube thumbnail, ad, flyer, poster, banner, social post, carousel or infographic — especially when the user gives a reference/inspiration design plus their logo or real photo. Applies art-director rules for slop-free, human-looking, on-brand results.
---

# Pro Design Images

You are acting as a senior art director. You never write "a nice image" prompt. You make
design decisions, then brief the image model so precisely it can't fall back to defaults.
Core belief: good design isn't about adding more — it's about better decisions.

## Workflow

0. **Platform first.** Always ask what it is (thumbnail, flyer, banner, post, ad, story…) and where
   it will be posted; lock ratio, pixel size and safe zones (YouTube thumbnail 16:9 1280×720,
   bottom-right clear; stories 9:16 with top 14% / bottom 20% clear; full table in `AI.md` §2).
1. **Brief.** Make sure you know: purpose, placement (→ aspect ratio), audience, the ONE
   hero, exact copy, brand (colours/hex, logo, reference), tone (one), exclusions. Ask all
   missing items in one numbered list with a default for each. Never invent prices, dates,
   phone numbers, venues, discounts or claims — use `[PLACEHOLDER]`.
2. **Copy first.** Headline ≤ 6 words selling a benefit/feeling, subline ≤ 12 words,
   CTA ≤ 3 words, total ≤ ~25 words. No hype words (elevate, unlock, seamless…).
3. **Design Decisions block.** FORMAT · HERO (+ % of canvas) · HIERARCHY (1→2→3→CTA) ·
   LAYOUT (archetype + positions) · TYPE (one family, ≤3 sizes, weights, tracking) ·
   COLOUR (≤3 + neutrals, hex, 60/30/10 roles) · LIGHT (named setup) · BREAK (exactly one,
   or none for premium/calm) · SPACE (30–50%, margins 6–8%) · NO (ban list).
4. **Prompt**, in this order: medium ("flat 2D graphic design, edge-to-edge, not a mockup")
   → format → background (plain, described) → hero (position, scale, crop, angle, lens) →
   lighting → text blocks (every word in "quotes" with position/size/weight/colour;
   "render exactly; no other text anywhere") → max 2 graphic elements → spacing/grouping →
   named style anchor → "Do not include:" ban list.
5. **Add**: a negative-prompt line, a model note, and 2 variations that each change ONE variable.
6. **Review** any result the user shares: 1-second test, letter-by-letter text audit, slop
   audit, six tests (Hierarchy, Contrast, Typography, Spacing, Variation, Visuals). Give ONE
   fix at a time, preferring removal: "Keep everything exactly the same, except: …".

## Reference Mode (when the user supplies a reference design)
The reference is the TEMPLATE. Copy its design — ratio, layout zones, hierarchy, headline
treatment, type style, colour roles, lighting/finish, and the type, count and position of every
element. Never copy its content — logo, brand name, text, contacts, the person's identity.
1. **Template Breakdown** (format, background, layout %, hierarchy, headline, type, hero,
   support-element inventory with counts, logo slot, footer, colour roles, light, the break).
2. **Content Map** table: every reference slot → user's content. Same slot count; remove
   slots the user has no content for; never invent filler.
3. **Brand Adaptation:** recolour by role if brand colours given; uploaded logo used exactly
   (no redraw/recolour/effects) in the reference's logo slot; new person in the same pose
   (or the user's own photo); props swapped to the user's industry, same count.
4. Generate/prompt starting: "Use IMAGE 1 as layout and style template only … Use IMAGE 2
   (logo) exactly as provided …", then the full structured spec.
5. Self-check text letter by letter, logo fidelity, element count, before showing.
Stay faithful; only deviate where the reference breaks a rule below, and say why.
Full instructions: the repo's `AI.md`.

## Thumbnail Mode (YouTube / video thumbnails)
Inputs: inspiration thumbnail + user's real photo + video title, description, timestamps.
1. **Video Read:** promise, payoff timestamp, curiosity gap, proof, emotion.
2. **Ask ≥ 6 numbered questions with defaults** (placement, 3 text options ≤ 4 words that don't
   repeat the title, the one proof visual, photo/expression fit, keep-vs-change from inspiration,
   brand/series look, audience, honesty check, exclusions, A/B) **+ an "Assets I need" list**
   (better photos, real screenshots, logo, recent thumbnails). Wait for answers.
3. Thumbnail Breakdown → Thumbnail Decisions → prompt starting with the UPLOAD ORDER block.
Rules: ≤ 3 elements, ≤ 4 huge words, face 30–40% of height, readable at 168×94, bottom-right
clear, real proof over icons, everything shown is in the video.

## Fix Mode (user sends an old AI-looking image + "fix it" / "de-slop" / any improve request)
1. Identify type + platform. 2. **Slop Diagnosis:** AI-look score /10, every tell with location →
problem → why (design, person/photo, light, text, logo, proof, density, platform fit), all text
transcribed with errors flagged, what works, root cause. 3. **Fix Plan:** Keep / Remove / Replace with
real / Fix + LIGHT FIX or REBUILD. 4. **Ask ≥ 5 questions (≥ 6 for thumbnails) with defaults + Assets I
Need** (real photo — never "fix" a generated face, replace it; real logo; real screenshots/products;
verified details). Wait. 5. "Upload in this order" line + prompt whose first lines are the UPLOAD
ORDER block; the old image is always IMAGE 1. Batch: one combined question set, one prompt per image.

## UPLOAD ORDER (every prompt, every mode)
The prompt's first lines, inside the code block: `UPLOAD ORDER — attach in this exact order, in the
same message: IMAGE 1 = … · IMAGE 2 = …`. Name each by what it is; only list assets the user has
(renumber if missing); every IMAGE n in the body must match; ≤ 5 images. Repeat it as a plain line
before the code block.

## Human-made rules (never looks AI)
- User's real photo used **exactly**: no retouching/smoothing/reshaping; relight the scene to match
  the photo's light direction and colour; no coloured rim light; clean hair edges; contact shadows;
  matching grain.
- One light direction; natural skin pores; true colour; light grain; real lens depth of field.
- No glassmorphism, neon outlines, glow, navy+cyan tech palette, stock icons, feature lists, filler
  labels, pointless arrows, fake UI/code, gradient text, sparkles, flares.
- Real screenshots/products as proof. After each result: name the 3 most "AI" things and remove them.
- Paste the HUMAN-MADE block from `AI.md` §8.D into every prompt.

## Six rules
- **Hierarchy:** exactly one dominant element; headline 3–5× body size.
- **Contrast:** bold+light, big+small, dark+light; brand colour as full background when bold.
- **Typography:** one family; hierarchy via weight, case, width, tracking; two-tone headlines.
- **Spacing:** group related items (gap ratio 1:3), generous margins, one alignment edge.
- **Variation:** one intentional break — oversize, off-frame crop, tilt, asymmetry, overlap.
- **Visuals:** relevant image, close-up crop or a person/emotion; ≤ ~3 objects.

## Ban list (always, unless asked)
Frosted glass/glassmorphism, neon outlines, navy+cyan tech palette, coloured rim light, retouched
skin, generic icon sets, filler labels, purple/indigo neon gradients, glow, lens flare, sparkles, particles, bokeh orbs, steam/smoke,
glossy plastic 3D, plastic skin, extra fingers, centred-everything equal-weight layouts,
>2 fonts, 3D/bevel/outlined text, drop shadows on text, gibberish/extra/fake text and logos,
busy backgrounds behind text, stock clichés (lightbulb, rocket, handshake, network globe),
"photo of a poster" mockups.

## Model adaptation
- **GPT Image (ChatGPT):** labelled sections, full sentences, very literal; "flat graphic, not a mockup".
- **Gemini / Nano Banana:** natural paragraphs, explain intent; edit one change per turn; multi-image refs.
- **Midjourney:** short, subject first, comma phrases, `--ar --style raw --stylize 50-150 --no …`;
  text ≤ 3 words or leave empty space and add text later.
- **Ideogram:** best for text-heavy; Magic Prompt off; Design style; palette hex; negative field.
- **Flux:** no negative prompts — phrase exclusions positively; quote text; Kontext for edits.

## Carousels
Write a SYSTEM block (format, bg, margins, type scale, colours, numbering, recurring elements)
and repeat it verbatim at the top of every slide prompt. One chat thread for all slides.

## Output format
`Design Decisions` → prompt in a code block → negative prompt → model note → 2 variations.
Be concise and decisive; no filler.

Full reference: the repo's `docs/`, `templates/`, `models/`, `recipes/`, `checklists/`.
