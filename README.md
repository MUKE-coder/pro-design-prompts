# Pro Design Prompts — Stop AI Slop, Generate Pro-Grade Designs

A playbook that turns any image AI (ChatGPT / GPT Image, Gemini / Nano Banana, Midjourney,
Ideogram, FLUX…) into a **detail-obsessed senior art director** — so your flyers, posters,
product ads, promos and carousels look designed, not generated.

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

Full explanations with before/after diagnoses: [docs/01-six-principles.md](docs/01-six-principles.md)

---

## Quick start (2 minutes)

1. Open ChatGPT, Gemini or any chat model.
2. Paste the box from **[SYSTEM_PROMPT.md](SYSTEM_PROMPT.md)** (or save it as Custom
   Instructions / a Gem / a custom GPT / a Project).
3. Say what you need: *"Flyer for a gospel concert, 14 Dec, Kampala Serena, 6 PM, free entry."*
4. Answer its quick questions → get **Design Decisions + a model-specific prompt + negative prompt + 2 variations**.
5. Generate ~4, pick the closest to the brief, **edit by removing**, run the
   **[checklist](checklists/pre-publish.md)**, post.

Prefer filling blanks? Use a **[template](templates/)**.
Using an AI agent (Claude, etc.)? Load the **[skill](skill/pro-design-images/SKILL.md)**.

---

## What's inside

```
SYSTEM_PROMPT.md                  ← the master "art director" prompt (paste this)
docs/
  01-six-principles.md            ← hierarchy, contrast, type, spacing, variation, visuals
  02-ai-slop-tells.md             ← the ban list + negative prompts + the deletion pass
  03-layout-and-composition.md    ← formats/ratios, grid in words, layout archetypes, camera
  04-typography.md                ← type scale, font vocabulary, getting text to render right
  05-colour-and-light.md          ← 60/30/10, palettes with hex, lighting setups, anti-plastic
  06-copy-and-text.md             ← voice, text budget, headline formulas, no invented facts
  07-workflow.md                  ← brief → decide → rounds → delete → check → save recipe
models/                           ← GPT Image, Gemini/Nano Banana, Midjourney, Ideogram/Flux
templates/                        ← product ad, event flyer, business promo, carousel, infographic
examples/slop-vs-pro.md           ← 7 bad prompts rewritten as pro prompts
recipes/                          ← 10 reusable style recipes (Hot Sale, Worship Night, …)
checklists/pre-publish.md         ← run before every post
skill/pro-design-images/SKILL.md  ← agent skill version (Claude / Cowork / Claude Code)
```

---

## The anatomy of a pro prompt

```
[1] Medium      "Flat 2D social ad design, edge-to-edge, not a mockup"
[2] Format      4:5 portrait
[3] Background  one plain colour / two-tone gradient — described, not decorated
[4] Hero        subject + position + scale (%) + crop + angle + lens
[5] Light       named setup (key / fill / rim)
[6] Text        every word in "quotes" + position + size + weight + colour; "no other text"
[7] Graphics    max 2 (pill button, badge, divider)
[8] Spacing     margins, groups, % empty space
[9] Anchor      named style reference, not "modern/clean"
[10] Exclusions "Do not include: …" ban list
```

## Golden rules

- **Decide, don't describe.** "Headline 15% of height, extra-bold condensed, top-left" beats "bold modern text".
- **One hero. One break. One family.**
- **Quote every word.** Never let the AI invent prices, dates, phone numbers or venues.
- **Edit by deleting.** Removing things fixes more than adding.
- **Heavy text? Go hybrid** — generate the visual with empty space, set text in Canva/Figma.
- **Real logo, real product photo** whenever trust matters. Never ship an AI-drawn logo.

---

## Credits & further reading

- The six principles are adapted from a before/after design carousel by **@gg.designhub** on Instagram.
- [Avoiding AI Slop — UI UX Pro Max](https://ui-ux-pro-max-skill.com/blog/avoiding-ai-slop/) — anchor to references, ban the tells, one strong decision, iterate by deleting.
- [Avoid AI Slop: a guide for marketers & PR — Merritt Group](https://www.merrittgrp.com/mg-blog/avoid-ai-slop-guide-for-marketers-and-pr/) — negative constraints, explicit voice, human review.
- [How not to create AI slop — AIVA](https://www.aiva.ie/blog/how-not-to-create-ai-slop) — brief first, exclusions, generate in rounds, text handling, pre-publish checklist.

Brand names in the docs describe the reference carousel or serve as style anchors. Use your
own brand assets in real work, and respect trademarks.

## License
MIT — use it, fork it, improve it. PRs with new recipes and templates welcome.
