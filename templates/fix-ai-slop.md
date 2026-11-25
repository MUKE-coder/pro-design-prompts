# Template: Fix an Old AI-Looking Image ("FIX IT")

Got thumbnails, flyers or posts that scream "AI made this"? Send one and say **FIX IT**.

```text
Read and follow: https://raw.githubusercontent.com/MUKE-coder/pro-design-prompts/main/AI.md

FIX IT — Image 1 is my old design.
[optional: it's a YouTube thumbnail / flyer / banner · posted on … · what bothers me: …]
```

Any wording works: "fix it", "de-slop this", "make it look real", "remove the AI look", "redo this".
Already loaded the link earlier in the chat (or using the Custom GPT / Gem)? Just send the image +
**FIX IT**.

## What happens

1. **Slop Diagnosis** — an AI-look score /10, every tell with its location ("right side → airbrushed
   skin + cyan rim light"), all the text it can read (with misspellings flagged), what's worth keeping,
   and the root cause.
2. **Fix Plan** — Keep / Remove / Replace-with-real / Fix, and a fix level:
   **LIGHT FIX** (keep the layout, edit the image) or **REBUILD** (layout is the problem, redesign it).
3. **Questions + Assets I Need** — at least 5 questions (6 for thumbnails), each with a default, plus
   exactly which real files to send (your photo, logo, screenshots, product photos…) and why.
   Reply `ok`, or e.g. `1 ok, 2 rebuild, 3 phone is 0772 123 456`, and attach the assets.
4. **The fix prompt**, with the upload order spelled out twice — once as a line for you, and once at
   the top of the prompt itself:

```text
UPLOAD ORDER — attach these images in this exact order, in the same message as this prompt:
IMAGE 1 = my old design (the one to fix)
IMAGE 2 = my real photo
IMAGE 3 = my logo
IMAGE 4 = real screenshot of the dashboard

Fix IMAGE 1. Keep its layout … Change only the following: …
```

5. Open ChatGPT (or Gemini), **attach the images in that exact order**, paste the prompt, send.

> The old image is always **IMAGE 1**. If you don't have an asset, say so — it's dropped from the
> list and the numbers shift, so the prompt never points at an image you didn't attach.

## Fixing many images at once
Send several images with **FIX ALL**. You'll get a short diagnosis of each, one combined set of
questions and assets (your photo and logo are reused), then one prompt per image — each with its own
upload order — plus a style recipe so the whole set looks consistent.

## Follow-ups

| Problem in the fixed result | Say |
|---|---|
| Face still looks generated | "My face was changed. Use IMAGE 2 exactly — no retouching. Change nothing else." |
| Some tells survived | "Human-made audit again: name the 3 most AI-looking things left and remove them. Keep everything else." |
| Text wrong | "Only change the text "…" to "…". Keep everything else identical." |
| Still feels like the old one | "Switch to REBUILD." |
