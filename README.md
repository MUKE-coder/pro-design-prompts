# Pro Design Prompts — Stop AI Slop, Generate Pro-Grade Designs

A playbook that turns any image AI (ChatGPT / GPT Image, Gemini / Nano Banana, Midjourney,
Ideogram, FLUX…) into a **detail-obsessed senior art director** — so your flyers, posters,
YouTube thumbnails, banners, product ads and carousels look **designed and shot by a human** —
not generated.

> **AI slop isn't "made with AI". It's made without decisions.**
> This repo replaces every vague adjective with a design decision.

---

## The six principles

| # | Principle | In one line |
|---|---|---|
| 1 | **Hierarchy** | One element is the boldest. Everything else recedes. |
| 2 | **Contrast** | Bold + light, big + small, dark + light. Stop playing it safe. |
| 3 | **Typography** | One strong typeface. Hierarchy from weight, size, case and tracking. |
| 4 | **Spacing** | Group related things. Leave 30–50% breathing room. |
| 5 | **Variation** | One intentional pattern-break: oversize, crop, tilt, asymmetry. |
| 6 | **Visuals** | A relevant image, close-up or emotion — not a wall of text. |
| + | **Human-made** | Real photo untouched, light matched, no glass/glow/stock icons — nobody thinks "AI". |

Full explanations with before/after diagnoses: [docs/01-six-principles.md](docs/01-six-principles.md)

---

## Quick start — just paste the link

The AI always asks first: **what are you making, and where will you post it?** (YouTube thumbnail,
flyer, banner, Instagram, WhatsApp status, print…) — then locks the right size and safe zones.

### YouTube thumbnail
Attach **(1) an inspiration thumbnail**, **(2) your real photo**, (3) optional screenshots/logo, then send:

```text
Read and follow: https://raw.githubusercontent.com/MUKE-coder/pro-design-prompts/main/AI.md

Making: YouTube thumbnail   Posting on: YouTube
Image 1 = inspiration. Image 2 = my real photo.
Video title: ...
Description: ...
Timestamps: ...
```
The AI reads your video, asks **at least 6 questions** (with defaults — reply "ok") and asks for any
extra assets it needs, then gives you the prompt plus the order to attach the images in ChatGPT.
Full message: **[templates/youtube-thumbnail.md](templates/youtube-thumbnail.md)**.

### Fix an old AI-looking image
Attach the old thumbnail/flyer and send:
```text
Read and follow: https://raw.githubusercontent.com/MUKE-coder/pro-design-prompts/main/AI.md

FIX IT — Image 1 is my old design.
```
You get a **Slop Diagnosis** (score, every tell and where it is), a keep/remove/replace plan, questions
plus the real assets to send, then a fix prompt that opens with the **UPLOAD ORDER** — your old image
is always IMAGE 1. Full guide: **[templates/fix-ai-slop.md](templates/fix-ai-slop.md)**.

> Every prompt this repo produces starts with an **UPLOAD ORDER** block, so you always know which
> image to attach first, second, third.

### Flyer, banner, ad or social post

In ChatGPT or Gemini, attach **(1) a reference design you like** and **(2) your logo**, then send:

```text
Read and follow: https://raw.githubusercontent.com/MUKE-coder/pro-design-prompts/main/AI.md

Making: flyer   Posting on: Instagram feed + WhatsApp status
Image 1 = reference template. Image 2 = my logo.
Company: ...   Headline: ...   Services: ...   Phone: ...   Brand colours: ...
```

The AI reads **[AI.md](AI.md)** (one self-contained instruction file), then:
1. **Breaks down the reference** — layout, headline treatment, every element and its count, colours, lighting.
2. **Maps your info into each slot** — never copies the reference's text, logo, contacts or person.
3. **Applies your brand** — recolours by role, places your logo exactly as uploaded.
4. **Generates the design** while enforcing every rule below, checks every letter, and gives you the reusable prompt.

No reference image? Just describe the job — it switches to Brief Mode and asks you 8 quick questions.

Full fill-in message + follow-up commands: **[templates/from-reference.md](templates/from-reference.md)**.

> **Design every week? Set it once:** paste the contents of `AI.md` into a **Custom GPT** (ChatGPT) or a
> **Gem** (Gemini). Then you never paste anything — just open it and drop your images.
> If ChatGPT can't open the link, turn on web search or attach `AI.md` as a file.

Prefer filling blanks without a reference? Use a **[template](templates/)**.
Using an AI agent (Claude, etc.)? Load the **[skill](skill/pro-design-images/SKILL.md)**.

---

## What's inside

```
AI.md                             ← THE file the AI reads from the link (all modes + rules)
SYSTEM_PROMPT.md                  ← how to load AI.md + a short paste-in version
docs/
  01-six-principles.md            ← hierarchy, contrast, type, spacing, variation, visuals
  02-ai-slop-tells.md             ← the ban list + negative prompts + the deletion pass
  03-layout-and-composition.md    ← formats/ratios, grid in words, layout archetypes, camera
  04-typography.md                ← type scale, font vocabulary, getting text to render right
  05-colour-and-light.md          ← 60/30/10, palettes with hex, lighting setups, anti-plastic
  06-copy-and-text.md             ← voice, text budget, headline formulas, no invented facts
  07-workflow.md                  ← brief → decide → rounds → delete → check → save recipe
  08-reference-mode.md            ← reference image → your brand, with a full worked example
  09-human-made-look.md           ← why people can tell it's AI, and the rules that stop it
  10-thumbnails.md                ← YouTube thumbnail workflow, specs, rules, photo tips
models/                           ← GPT Image, Gemini/Nano Banana, Midjourney, Ideogram/Flux
templates/                        ← fix-ai-slop, youtube-thumbnail, from-reference (start here), product ad, event flyer,
                                    business promo, carousel, infographic
examples/slop-vs-pro.md           ← 8 bad prompts rewritten as pro prompts (incl. a thumbnail)
recipes/                          ← 10 reusable style recipes (Hot Sale, Worship Night, …)
checklists/pre-publish.md         ← run before every post
skill/pro-design-images/SKILL.md  ← agent skill version (Claude / Cowork / Claude Code)
```

---

## The anatomy of a pro prompt

```
[0] Platform    what it is + where it's posted → ratio, size, safe zones
[1] Medium      "Flat 2D social ad design, edge-to-edge, not a mockup"
[2] Format      e.g. 16:9 1280×720 thumbnail · 4:5 portrait feed
[3] Background  one plain colour / two-tone gradient — described, not decorated
[4] Hero        subject + position + scale (%) + crop + angle + lens
[5] Light       named setup (key / fill / rim)
[6] Text        every word in "quotes" + position + size + weight + colour; "no other text"
[7] Graphics    max 2 (pill button, badge, divider)
[8] Spacing     margins, groups, % empty space
[9] Anchor      named style reference, not "modern/clean"
[10] Human-made real photo untouched, one light direction, no glass/glow/stock icons
[11] Exclusions "Do not include: …" ban list
```

## Golden rules

- **Decide, don't describe.** "Headline 15% of height, extra-bold condensed, top-left" beats "bold modern text".
- **One hero. One break. One family.**
- **Quote every word.** Never let the AI invent prices, dates, phone numbers or venues.
- **Edit by deleting.** Removing things fixes more than adding.
- **Heavy text? Go hybrid** — generate the visual with empty space, set text in Canva/Figma.
- **Real logo, real product photo, real face** whenever trust matters. Never ship an AI-drawn logo.
- **Change the scene, not the face.** Your photo is used exactly; the background is relit to match it.

---

## Credits & further reading

- The six principles are adapted from a before/after design carousel by **@gg.designhub** on Instagram.
- [Avoiding AI Slop — UI UX Pro Max](https://ui-ux-pro-max-skill.com/blog/avoiding-ai-slop/) — anchor to references, ban the tells, one strong decision, iterate by deleting.
- [Avoid AI Slop: a guide for marketers & PR — Merritt Group](https://www.merrittgrp.com/mg-blog/avoid-ai-slop-guide-for-marketers-and-pr/) — negative constraints, explicit voice, human review.
- [How to de-slopify your designs — UX Collective](https://uxdesign.cc/how-to-de-slopify-your-designs-4c40c57c1dc9) — glassmorphism, default styling, high density; reflect, remove, choose deliberately.
- [How not to create AI slop — AIVA](https://www.aiva.ie/blog/how-not-to-create-ai-slop) — brief first, exclusions, generate in rounds, text handling, pre-publish checklist.

Brand names in the docs describe the reference carousel or serve as style anchors. Use your
own brand assets in real work, and respect trademarks.

## License
MIT — use it, fork it, improve it. PRs with new recipes and templates welcome.
