# Template: Event Flyer / Poster

Concerts, church events, conferences, parties, graduations, launches.
Events carry the most text — be strict about hierarchy. **Event name or headliner is the hero.**

## Collect the facts first (never let AI invent these)
```text
EVENT NAME:   [ ]
KICKER:       [e.g. "SUNDAY 14 DECEMBER 2026" or "LIVE IN KAMPALA"]
HEADLINER(S): [ ]   (use an uploaded photo for real people — don't let AI invent faces of real artists)
DATE · TIME:  [ ]
VENUE:        [ ]
PRICE/ENTRY:  [e.g. "Ordinary UGX 20,000 · VIP UGX 50,000" / "Free Entry"]
CONTACT/CTA:  [phone / "Tickets: [website]" / QR placeholder]
SPONSORS:     [leave an empty strip at the bottom — add logos later in Canva]
```

## Design Decisions
```text
FORMAT:     [2:3 / A4 print] or [4:5 feed] or [9:16 status]
HERO:       [event name as giant type] OR [headliner photo, 60% of canvas]
HIERARCHY:  1 [event name] → 2 [date] → 3 [headliner/visual] → 4 [venue·time·price] → 5 [CTA]
LAYOUT:     [Typographic poster / Full-bleed photo with text in calm area / Headline-top hero-bottom]
TYPE:       [display face for headline] + [one clean sans for details]
COLOUR:     [bg #hex] · [accent #hex] · [text #hex]
LIGHT:      [single warm beam from top / stage spotlight / golden hour]
BREAK:      [headline so large it's cropped by the edges / photo subject overlaps headline]
SPACE:      40% calm; bottom 12% reserved for sponsor logos
NO:         [ban list]
```

## Prompt
```text
Create a flat 2D event poster design, edge-to-edge, [2:3 portrait]. Not a mockup.

BACKGROUND: [deep navy #0E1A3A] with [one soft warm-gold light beam coming from the top
centre]. Subtle [film grain] texture. Nothing else.

HERO: [Typographic: the event name is the image — huge type filling the middle 60% of the
canvas] OR [a single [performer/person] photographed from a low angle with an 85mm lens,
stage spotlight from above, natural skin texture, positioned centre-right, the top of their
head overlapping the bottom of the headline letters].

TEXT — render exactly as written, correct spelling, no other text anywhere:
- Top, small, [gold] all-caps, wide letter-spacing: "[KICKER]"
- Below, VERY LARGE, [elegant high-contrast serif / ultra-condensed bold sans], [cream],
  [2] lines, tight leading: "[EVENT NAME LINE 1]" / "[LINE 2]"
- [Small line under headline: "featuring [NAME]"]
- Bottom-left block, small clean sans-serif, [cream], 3 lines, left-aligned:
  "[VENUE]" / "[DATE] · [TIME]" / "[PRICE]"
- Bottom-right, small [gold pill button]: "[CTA e.g. Call 0700 000 000]"
- Leave the bottom 12% as an empty [darker] strip for sponsor logos.

LAYOUT: 8% margins; one left alignment edge for details; strong size jump between headline
and details; 40% calm empty space.

STYLE: [premium gospel concert poster / modern music festival poster / corporate conference
key visual]. Minimal, confident, intentional.

DO NOT INCLUDE: doves, crosses, clip-art, sparkles, glitter, lens flares, smoke, multiple
fonts, outlined text, 3D text, drop shadows, fake logos, extra text, busy patterns, collage.
```

## Text-heavy? Use the hybrid route
Generate with the **detail areas empty** ("leave the bottom third empty for text"), then set
venue/date/price in Canva or Figma using your type specs. Zero typos, fully editable.
