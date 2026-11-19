# Model Guides — Which Model for Which Job

Model versions change every few months (late 2026: GPT Image 2.x in ChatGPT, Nano Banana 2 / Pro
in Gemini, Midjourney V8.x, Ideogram 4.x, FLUX.2 / Flux 3). The **principles in this repo don't
change** — only the prompt *format* does. Check your tool's current version and docs.

| Job | First choice | Why | Backup |
|---|---|---|---|
| Text-heavy flyer / poster (dates, venue, prices) | **Ideogram** or **ChatGPT (GPT Image)** | Most reliable text rendering | Gemini Nano Banana Pro |
| Product ad with 1 headline | **ChatGPT** or **Gemini** | Follows layout instructions literally, good text | Ideogram |
| Editing a result ("keep everything, change X") | **Gemini (Nano Banana)** or **ChatGPT** | Conversational editing keeps the rest intact | Flux Kontext |
| Moody, artistic, editorial visual | **Midjourney** | Best raw aesthetic taste | Flux |
| Photoreal people & products | **Gemini Nano Banana Pro** or **FLUX** | Realistic skin/materials | GPT Image |
| Carousel series (consistent look) | **ChatGPT** or **Gemini** in one chat thread | Remembers the system across slides | Ideogram with style reference |
| Using YOUR real product photo | **Gemini** or **ChatGPT** (upload it) | Image-to-image editing | Flux Kontext |

**Pro combo:** Midjourney for the hero visual (with empty space for text) → upload to ChatGPT/Gemini/Ideogram
to add exact text → final check in Canva/Figma.

Guides:
- [gpt-image.md](gpt-image.md) — ChatGPT / OpenAI GPT Image
- [gemini-nano-banana.md](gemini-nano-banana.md) — Google Gemini / Nano Banana
- [midjourney.md](midjourney.md)
- [ideogram-flux-others.md](ideogram-flux-others.md) — Ideogram, FLUX, Recraft, Firefly, Leonardo, Seedream
