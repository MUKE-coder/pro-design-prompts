# The Pro Workflow: Brief → Decide → Generate in Rounds → Delete → Check

Slop is usually **"one prompt, first result, posted."** Pros work in rounds.

```
 1. BRIEF      8 answers (purpose, placement, audience, one thing, copy, brand, tone, exclusions)
 2. DECIDE     Design Decisions block (hero, hierarchy, layout, type, colour, light, break, space)
 3. PROMPT     Structured prompt + negative prompt
 4. ROUND 1    Generate ~4. Judge against the BRIEF, not beauty. Pick the closest.
 5. ROUND 2    Fix with specific edits — mostly REMOVING things.
 6. ROUND 3    Small adjustments (text fix, crop, colour). Then STOP.
 7. CHECK      Pre-publish checklist. Any fail → fix or discard. Never "close enough".
 8. SAVE       Turn the winner into a named Style Recipe for reuse.
```

---

## Round 1 — judge against the brief

Score each of the 4 results quickly:
- Is the hero the first thing I see? (Y/N)
- Is the text correct? (Y/N)
- Any ban-list items? (count)
- Right ratio / text-safe areas? (Y/N)

Pick the best one. If none is close, the **prompt** is wrong — change the Design Decisions, not just words.

## Round 2 — edit, don't re-roll

On editing-capable models (ChatGPT, Gemini, Ideogram, Flux Kontext, Midjourney Editor):
```text
Keep everything exactly the same — layout, text, product, colours, lighting — except:
1. Remove the sparkles around the can.
2. Make the headline 30% larger.
3. Replace the patterned background with a solid #0B2A6F.
```
- Max 3 changes per edit. One is best.
- Removing > adding. Adding is how slop happens.

## Round 3 — polish, then stop

- Fix any wrong letter: "Only change the text 'Shpo Now' to 'Shop Now'. Keep everything else identical."
- Crop for the platform.
- Upscale for print.
- If text still fails after 2 tries → remove the text and add it in Canva/Figma.

## Save a Style Recipe

Ask the model:
```text
Describe the visual style of this image as a reusable "style recipe" in 60–90 words:
palette with hex, typography style, layout archetype, lighting, background, texture,
and what it never includes. Name it. Do not describe the subject.
```
Store it in `recipes/`. Next time: `Use this style: [recipe]. New subject: [...]`.
Keep 3–4 recipes per brand for consistency across posts.

## Swipe file

Keep a folder of designs you love **and** hate, each with one line: *why*.
Use them to describe **style**, not to copy subjects. Upload a loved one as a style reference
(Midjourney `--sref`, Ideogram style reference, ChatGPT/Gemini "match the style of this image").

## Real photos first (when trust matters)

For real food, real faces, real venues and real products customers will recognise, a real
photo usually builds more trust. Use AI for layout, backgrounds, concepts, moods, and series
consistency — then composite your real product photo in, or upload it and ask the model to
design around it ("Use the uploaded product photo exactly as is; do not redraw the product").
