# Photoshop Master: Think in Layers, Not Prompts

An AI image looks like AI because nothing in it has a *cause*. The glow isn't coming from anything,
the shadows point different ways, the face was never photographed, the edges were never masked.

A Photoshop masterpiece is the opposite: every pixel comes from a **real asset**, a **mask**, a
**light**, a **shadow** or a **grade** that a designer chose on purpose. So the AI in this repo never
"just prompts". It first plans the PSD like a senior compositor, then asks the image model to render
that finished composite — or hands you the plan as steps to build it yourself.

The rules the AI follows are in [AI.md §14](../AI.md). This page explains them.

---

## 1. The PSD layer plan

Every job starts with a layer stack, bottom to top. Only the layers the design needs.

| # | Layer group | What a pro does there |
|---|---|---|
| 01 | Background | solid / texture / real photo / grid; a soft **light pool** behind where the subject will stand |
| 02 | Depth BG | shapes or giant type placed *behind* the subject; far things slightly defocused |
| 03 | Subject | real photo → Remove Background → Select & Mask for hair → remove colour fringe |
| 04 | Retouch | heal temporary spots, lint, dust · remove or clean props · light frequency separation (pores kept) · dodge & burn · subtle eye sharpening |
| 05 | Subject light | keep the photo's key light · add a **motivated** rim light on one side · contact shadows |
| 06 | Subject grade | curves + colour balance clipped to the subject so it matches the scene |
| 07 | Elements | cards, screenshots, products · smart-object mockups · stacked drop shadows |
| 08 | Logo / 3D | real logo · optional clean extrusion/bevel · same light angle |
| 09 | Type | font, size, colour · stroke / shadow / extrusion · overlap or knockout with subject |
| 10 | Finish | global gradient map or LUT (low opacity) · custom vignette · focus on subject · multi-level sharpen · film grain |

## 2. Technique library (what each move is for)

### Cut-outs & masks
- **Remove Background, then refine.** Automatic cut-outs miss hair and leave coloured edges. Pros
  refine with Select & Mask, then remove the fringe left by the old background.
- **Smooth edges.** A bumpy mask edge is a giveaway; feather the mask slightly and add contrast back.
- **Check the mask.** Lower the mask density temporarily to see what was missed.

### Realistic retouching
- **Spot healing / clone / patch** — temporary blemishes, lint, dust, scratches, stray hairs.
- **Content-aware / generative fill** — remove a mic, a cable, a selfie arm, clutter; rebuild the
  sweater or wall behind it.
- **Light frequency separation** — even out blotchy tone while keeping every pore.
- **Dodge & burn** — shape the face and clothes with light and shadow; the most "pro" retouch move.
- **Colour fixes in skin** — target green or grey casts only.
- **Never:** reshape the face or body, change the expression, beauty-smooth the skin (see
  [09-human-made-look.md](09-human-made-look.md)).

### Light & depth
- **Background light pool** — a soft light behind the subject separates them from a dark background.
- **Motivated rim light** — a soft edge light on one side, in the colour of a light in the scene.
  A uniform cyan halo all around the person is the AI version; don't.
- **Stacked shadows** — a tight dark contact shadow plus a wide soft one makes floating cards and
  logos sit in real space.
- **One global light angle** — every shadow, bevel and highlight agrees. This alone kills most of the
  AI look.
- **Depth by overlap** — subject in front of the headline, an element tucked behind the head, far
  layers slightly blurred.

### Colour
- **Curves for punch** — brighter brights, darker darks, without crushing shadow detail.
- **Match subject to scene** — same black level, colour temperature and saturation.
- **Global grade** — a gradient map or colour lookup at 10–25% ties every layer together.
- **Flyer looks** — black-and-white subject with brand-colour accents, duotones, colour blocks.

### Graphic & type effects
- **3D logo or headline** — clean extrusion or bevel, real material (matte, metal, paper), same light
  angle as everything else.
- **Sticker stroke** — an even white or brand-colour outline around the cut-out subject.
- **Glow as light** — one element can glow *as if lit from behind*, in a palette colour. One.
- **Knockout & clipping** — text punched through a shape, a photo inside letters.
- **Type behind the subject** — giant headline with the subject overlapping it.

### Screens & mockups
- **Data UIs** (dashboards, apps, websites): placed exactly as captured, mapped onto devices like a
  smart object ([AI.md §8.G](../AI.md)).
- **Text-only screens** (terminal, code): a designer may **re-typeset** them in a better window —
  proper window chrome, good monospace font, real theme, depth — with every character identical.

### Integration check (never skip)
Light direction · light colour · black & white levels · contrast · saturation · grain · sharpness/blur
· perspective & horizon · edge quality · contact & cast shadows · reflections.
If one doesn't match, it looks pasted. Fix that before adding anything.

### Finishing
Custom vignette that keeps the lights bright · reduce shadows, exposure and clarity away from the
subject to pull focus · sharpen in levels (overall → face → eyes) · one fine grain over everything ·
smooth gradients (no banding) · check at thumbnail size and flipped horizontally.

## 3. Style playbooks

| Style | Photoshop moves |
|---|---|
| **Tech / YouTube thumbnail** | textured BG (grid/blueprint at low opacity) · cut-out subject with motivated rim light or sticker stroke · real logo as a 3D tile with stacked shadows · code chips re-typeset with connector lines · one glowing accent · gaze or gesture toward the topic |
| **Event / party flyer** | cut-out subject, often B&W with brand-colour accents · giant headline behind or around the subject · one script accent (≤ 2 words) + bold condensed sans · diagonal colour blocks · haze matched to the light · details in a tight bottom grid |
| **Product ad** | studio-lit real product · gradient sweep backdrop · contact shadow + soft reflection · floating laydown shadows · headline + price badge |
| **Portrait / personal brand** | dark seamless BG · rich, warm skin grade · dodge & burn · catchlights kept · subtle vignette · minimal type |
| **Corporate / clean** | light BG · soft stacked shadows · real UI mockups · one accent colour · lots of space |

## 3b. The WOW layer
Clean and real is the floor; a pro adds one idea you remember. See [AI.md §14.F](../AI.md) for the
WOW CONCEPT block, the signature moves (type lockups, subject in front of giant type, depth stacks
of real UI cards, light drama, designer's touches, story chips), the typography library with named
fonts, and the polish pass.

## 4. Worked example — Grit Framework thumbnail

**Test 2 result (the dark remake):** real face, real logo, all information kept — big step up. What
a Photoshop designer would still do:
- The terminal is a flat screenshot with a cyan border → **re-typeset** it as a designed terminal
  window (window chrome, monospace font, depth, tilt, stacked shadows), same exact command.
- The subject is lit flat and sits *on* the background → background light pool behind him, a soft
  **motivated** blue rim light on one side (from the same blue as the logo), dodge & burn, a subject
  grade that matches the navy scene.
- The logo is flat → a clean **3D tile** with a matte finish and stacked shadow, same light angle.
- No depth → a faint blueprint grid behind, slightly defocused; the terminal overlapping his chest;
  the card casting a shadow on the backdrop.
- The arrow now points at one row again → point it at the card.

**PSD layer plan**
```
01 BACKGROUND   navy #0B1220, faint blueprint grid at 8% opacity fading toward the edges, soft
                light pool (#1E3A6E, Screen) behind the head
03 SUBJECT      real photo · BG removed · hair refined · selfie arm removed
04 RETOUCH      mic cleaned (same model) · forehead shine reduced · dodge & burn on cheekbones,
                jaw, sweater folds · eyes subtly sharpened · pores kept
05 LIGHT        key light from the photo · soft #3DB5F5 rim light on his right edge only (motivated
                by the blue light pool) · contact shadow under the mic
06 GRADE        subject curves to match navy black level, slight cool shift in shadows
07 ELEMENTS     feature card: solid #111827, 1px #24324F border, stacked shadows (global light 120°)
                terminal: re-typeset in a dark window (title bar, 3 dots, JetBrains Mono, Git Bash
                colours), tilted 4° in perspective, overlapping his chest, stacked shadows
08 LOGO         real logo as 3D tile, 18px matte extrusion, soft shadow at 120°
09 TYPE         "Grit Framework" white, subtle 2px darker-navy extrusion; subtitle flat
10 FINISH       gradient map navy→warm white at 12% Soft Light · custom vignette · high-pass sharpen
                on face/eyes · fine grain over everything
```

## 5. Build it by hand (Photopea / Photoshop recipe)

When the image model keeps changing the face or the text, ask the AI for the **PSD recipe**. You get
numbered steps like:
1. New 1280×720 document, fill #0B1220. Add Noise 2%, monochromatic.
2. New layer, soft round brush #1E3A6E at 30% behind the head, blend mode Screen.
3. Place your photo → Remove Background → Select & Mask (Refine Hair) → Output: layer mask.
4. New layer above, clipped: Spot Healing on the mic and forehead shine (sample current & below).
5. 50% grey layer in Overlay: dodge (white 5%) cheekbones and nose bridge, burn (black 5%) jaw edge.
6. New layer, clipped, Screen: paint #3DB5F5 along his right edge only, 10–20% opacity.
7. Curves clipped to subject: lower blacks to match the background.
8. Type, logo, terminal, card — each with the same drop-shadow angle (Use Global Light on).
9. Gradient Map at 12% Soft Light, custom vignette, high-pass 1.5 px on face (Overlay, masked), grain.
10. Check at 168×94 and flipped horizontally. Export 1280×720 JPG under 2 MB.

Generate only what AI is good at (a background, a prop) and do the real photo, logo, text and
screens yourself — that's how pros use AI inside Photoshop.
