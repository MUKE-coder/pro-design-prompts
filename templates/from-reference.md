# Template: Reference Image → Your Brand (the copy-paste message)

This is the message you send to ChatGPT or Gemini. Attach the images **in this order**:
1. the reference design you like
2. your logo (PNG, transparent background if possible)
3. *(optional)* your own product photo or a photo of a real person to use

Then paste this and fill in the brackets (delete lines you don't need):

```text
Read and follow: https://raw.githubusercontent.com/MUKE-coder/pro-design-prompts/main/AI.md

Making: [flyer / poster / banner / social post / ad / story]
Posting on: [Instagram feed / WhatsApp status / Facebook / print A4 / website banner / …]

Image 1 = reference template. Image 2 = my logo. [Image 3 = my product/photo.]

Company: [Name]
What we do: [e.g. branding, posters, motion graphics, campaigns]
Headline: [e.g. "NEW WEEK" — or "suggest 3 options"]
Kicker / small line: [e.g. "IT'S A BRAND"]
Services / labels for the pills: [Branding, Posters, Motions, Illustrations, Campaigns]
Phone / WhatsApp: [+256 7XX XXX XXX]
Website / handle: [@yourhandle]
Brand colours: [#hex, #hex] — or "keep the reference colours"
Must not include: [anything]
```

**That's it.** (Making a YouTube thumbnail? Use [youtube-thumbnail.md](youtube-thumbnail.md).) The AI will:
0. confirm the platform and lock the size + safe zones
   …and (after the breakdown) pick a style playbook, a subject treatment (full colour / B&W with your
   brand accents / cut-out with stroke) and show the **PSD layer plan** it will brief — Photoshop-level
   work: cut-out, overlap with the headline, matched light and haze, stacked shadows, grade
1. break down the reference (layout, headline treatment, every element and its count, colours, lighting)
2. map your info into each slot (and ask about anything missing)
3. recolour by role if you gave brand colours
4. place your logo exactly as uploaded
5. generate the design, check every letter of your phone number, and give you the reusable prompt.

---

## Follow-up messages that work well

| You want | Say |
|---|---|
| Fix one thing | "Keep everything exactly the same, only change: [the phone number to +256 700 000 000]" |
| Logo got redrawn | "The logo is wrong. Use image 2 exactly as uploaded — do not redraw it. Change nothing else." |
| Too busy | "Remove the [3 smallest floating icons]. Keep everything else identical." |
| Different size | "Same design, re-laid out for 9:16 WhatsApp status. Keep text out of the top 14% and bottom 20%." |
| Colour version | "Same design in my brand colours [#hex, #hex] — recolour by role, keep contrast." |
| New week, same template | "Same template and logo. New headline: "[…]". New services: […]." |

## If ChatGPT says it can't open the link
- Make sure web search/browsing is on, then send the link again, **or**
- Use the GitHub page link instead: `https://github.com/MUKE-coder/pro-design-prompts/blob/main/AI.md`, **or**
- Download `AI.md` and attach it as a file with the message "Follow the instructions in AI.md", **or**
- **Set it once and forget it:** create a Custom GPT (ChatGPT) or a Gem (Gemini) and paste the content of
  `AI.md` into its instructions. Then you never paste anything again — just open that GPT/Gem and send
  your images. *(Recommended if you design every week.)*
