# Worked Example: Agency Flyer — Pinterest Template → Real, Polished, WOW

**Client:** Desishub (software agency, Kampala) · **Format:** Instagram/Facebook feed 4:5, 1080×1350
**Modes:** REFERENCE MODE → WOW PASS → targeted edit ([AI.md §4, §14.F](../AI.md))

![Final flyer](images/desishub-flyer-final.jpg)

*(Client names in the screenshots blurred for publication.)*

---

## 1. The inputs
- **Reference:** a Pinterest agency flyer (AI-generated: glossy 3D clay icons, purple→blue gradients,
  generated model, glowing petals, "!" headline). Used for layout only — not included here.
- **Brand facts:** company profile file (services, contacts, tone rules: plain English, British
  spelling, no exclamation marks, no "best/leading", monthly prices only with their minimum term).
- **Logo:** light version (blue D, navy "esis", red "hub").
- **Real proof:** three screenshots — a web POS system, a desktop property app, a web lending platform.
- **Person:** the user chose a generated model (a new person, photographic rules from §8.C).

## 2. The iterations — what each one taught the repo

| Round | What happened | Lesson → repo change |
|---|---|---|
| 1. Reference rebuild | Clean and real, but it copied the template too literally: equal petals, flat white, one generic font. "Lacks the wow." | **WOW layer (§14.F):** WOW CONCEPT, 1–3 signature moves, named-font typography library, polish pass |
| 1. (privacy) | The model **re-rendered blurred figures** as readable numbers | **§8.G:** blurred data doesn't stay blurred — capture demo-data screenshots for anything public |
| 2. WOW PASS | Giant "Software" with the model overlapping it, red serif sticker tag, real cards at depth, studio cyclorama + blue light pool. Big jump. But **original screenshots were uploaded** (browser tabs, client names visible) and **six elements vanished** (3 service chips, labels, status chip) | **Upload prepared files, not originals** · **CONTENT LOCK:** numbered "must contain" list at the end of long prompts |
| 3. Targeted edit | Chips, labels and the "Offline — still saving" story chip back; back card defocused for depth; most data blurred | ✅ Approved. One readable client name and a line of garbled small text were blurred by hand before publishing — always zoom into screenshot cards |

## 3. The WOW concept that worked
```
IDEA:        "She sits in front of the word she builds."
SIGNATURES:  1) giant "Software" with the model overlapping it  2) real UI cards at 3 depths
             3) red "that keeps working." sticker tag + an "● Offline — still saving" story chip
TYPE:        Bricolage Grotesque ExtraBold · Inter · Instrument Serif Italic (the tag only)
WORLD:       light-blue brand world + one red accent; soft key + blue light pool behind her
QUIET:       background, chips, footer
```

## 4. The two prompts
The WOW PASS prompt and the follow-up edit prompt are the ones in this repo's conversation log
pattern: §14.F WOW CONCEPT → §14.A layer plan → prompt with UPLOAD ORDER, PHOTOSHOP FINISH,
HUMAN-MADE, "Do not include" and a CONTENT LOCK. Key lines that made the difference:
```text
- "Software" — Bricolage Grotesque ExtraBold, #1F6BFF, huge: about 88% of the width, tracking −4%.
- She sits IN FRONT of the word: the top of her head overlaps only the bottom edge of the letters
  "twa", so the word stays fully readable.
- A red sticker tag stuck on the upper right of "Software", tilted −5°, "that keeps working." in
  white Instrument Serif Italic, with a small soft shadow, like a real sticker.
- Behind the chair on the right, slightly defocused (further away): the desktop app card.
- Any blurred areas must stay an unreadable soft blur — never invent names or figures.
Must contain all of these: 1 "We build" 2 "Software" 3 "that keeps working." … 11 the logo.
```

## 5. Final checks that caught problems
- Zoom into every screenshot card: client names, emails and figures; garbled small text.
- Count the content lock items.
- Same corner radius and shadow on every card and chip.

## 6. Reuse
Saved as the **DESISHUB CLEAN BLUE** recipe in [recipes/README.md](../recipes/README.md).
