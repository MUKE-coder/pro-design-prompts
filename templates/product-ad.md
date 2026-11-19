# Template: Product Ad / Social Post

Fill the `[BRACKETS]`. Delete lines you don't need. Keep the structure.

## Design Decisions (fill first)
```text
FORMAT:     [4:5 Instagram feed / 9:16 story / 1:1]
HERO:       [the product], about [50–70]% of canvas height
HIERARCHY:  1 [product] → 2 [headline] → 3 [offer/subline] → 4 [CTA]
LAYOUT:     [Split: text left 45%, product right 55% bleeding off the edge]
TYPE:       ONE family: [heavy condensed sans / rounded bold sans / neo-grotesk];
            headline [black weight, ~15% of height]; subline regular ~3%; CTA semibold
COLOUR:     background [#hex] 60% · secondary [#hex] 30% · accent [#hex] 10%
LIGHT:      [hard key from top-left + rim light / soft studio softbox]
BREAK:      [product oversized & tilted 15° / cropped by right edge / overlaps headline]
SPACE:      [35]% empty, 7% margins
NO:         [ban list]
```

## Prompt
```text
Create a flat 2D [social media advertisement] design, edge-to-edge, [4:5 portrait].
Not a mockup, not a photo of a poster.

BACKGROUND: [solid #hex / gradient from #hex to #hex, top to bottom / a single seamless
studio surface in #hex]. Nothing else in the background.

HERO: [PRODUCT DESCRIPTION — material, colour, key details]. It is [oversized, about 65% of
the canvas height], positioned [right half, bottom-aligned], [tilted 15° clockwise],
[cropped by the right edge]. Shot [low angle / eye level / front three-quarter] with a
[85mm] lens. Lighting: [LIGHT SETUP]. [Rim light separates it from the background.]

TEXT — render exactly as written, correct spelling, no other text anywhere:
- Headline, [top-left], [very large, ~15% of canvas height], [extra-bold condensed sans-serif],
  [white], [all caps], tight letter-spacing, [2] lines: "[HEADLINE LINE 1]" / "[LINE 2]"
- Subline below headline (close to it), small regular weight, [white at 85% opacity]:
  "[SUBLINE ≤ 12 words]"
- [Offer badge: a [yellow #hex] [tilted rectangle / circle sticker] reading "[Up to]" small
  and "[70% Off]" large]
- CTA, below with a larger gap, small [white pill button] with [dark] text: "[Shop Now →]"
- [Logo: leave an empty space top-left of 10% width for the logo] (add the real logo later)

LAYOUT: margins about 7% on all sides; all text left-aligned to one edge; headline and subline
grouped tightly; CTA separated; about [35]% calm empty background.

STYLE: [premium sportswear campaign / fast-food brand campaign / Apple-style product page]
art direction. High contrast, crisp, intentional, minimal.

DO NOT INCLUDE: sparkles, particles, lens flare, glow, purple gradient, splash, extra
products, props, fake logos, extra text, drop shadows on text, 3D text, clutter.
```

## Negative prompt
```text
sparkles, particles, lens flare, glow, neon, purple gradient, extra objects, clutter,
fake logo, watermark, gibberish text, extra text, drop shadow text, 3D text, mockup, frame
```

## Variations to test (change ONE thing)
- A: dark background version → swap background to `[#121212]`, text white.
- B: tighter crop → product 90% of height, cropped by top and right edges.
