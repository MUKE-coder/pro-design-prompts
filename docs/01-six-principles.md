# The Six Principles (Before → After)

These come from a before/after carousel by a professional designer. Each "before" is what
image AIs produce by default. Each "after" is what a pro makes. For every principle you get:
**the diagnosis**, **the rule**, and **the exact prompt language** that pushes the model toward the "after".

> "Good design isn't about adding more. It's about making better decisions."
> Hierarchy · Contrast · Typography · Spacing · Variation · Visuals

---

## 1. Give your design a clear hierarchy

**If everything looks equally important, nothing stands out.**

| Before (AI default) | After (pro) |
|---|---|
| Grey background, logo, title "Great Indian Festival Sale" in medium weight, paragraph, small button, boxes in corner. Everything the same visual weight. | Saturated orange background. "Great Indian Festival" is huge, white, extra-bold, stacked over 3 lines. A bright yellow badge says "Up to **70% Off**" — the second read. Small details line, white pill CTA. Boxes enlarged and cropped on the right edge. |

**Rules**
- Pick ONE first-read element. Write it in the prompt: *"The headline is the dominant element."*
- Headline 3–5× body size. Offer/number gets its own container (badge, sticker, pill).
- Define the reading order: **Hero → Headline → Offer → Details → CTA**.
- Supporting text smaller *and* lighter (lower weight or lower opacity).

**Prompt language**
```text
Clear visual hierarchy. First read: the headline "GREAT FESTIVAL SALE" in extra-bold
white sans-serif, stacked on three lines, occupying the top-left 55% of the canvas.
Second read: a tilted bright-yellow (#FFD400) rectangular badge reading "Up to 70% Off"
where "70% Off" is twice the size of "Up to". Third read: one small line of details.
Last: a small white pill button "Shop Now →". Nothing else competes with the headline.
```

---

## 2. Stop playing it too safe (Contrast)

**When everything has the same weight, size, or colour, your design feels flat.**

| Before | After |
|---|---|
| Off-white background, dark-grey title "Chicken Burger", small grey subline, burger centred. Low contrast. | Deep red (#C8102E) background, giant golden arch shape bleeding off the top-right. "Chicken" in white, "Burger" in brand yellow — two-tone headline. Burger is larger, overlapping the bottom edge, shot with appetising warm light. |

**Rules**
- Pair opposites: **bold + light**, **big + small**, **dark + light**, **saturated + neutral**.
- Use brand colour as a *full background*, not a timid accent.
- Two-tone headlines: split the headline across two colours or two weights.
- A big brand shape (cropped) adds energy without clutter.

**Prompt language**
```text
High contrast composition. Solid deep red background (#C8102E). Headline on two lines:
"Chicken" in bold white, "Burger" in bold golden yellow (#FFC72C), same extra-bold
rounded sans-serif. A single oversized yellow brand curve bleeds off the top-right
corner, cropped by the frame. The burger is large, front three-quarter view, warm key
light, crisp texture, cropped slightly by the bottom edge.
```

---

## 3. Make your type work harder

**Using more fonts won't automatically improve your design.** Choose one strong typeface,
explore weights, adjust letter spacing, create intentional sizes.

| Before | After |
|---|---|
| Light-grey card, italic title "Running Shoes", grey paragraph, grey rectangle button. Generic, forgettable. | Dark charcoal background with an orange light streak. "RUN FURTHER" in huge extra-bold italic condensed caps, tight tracking, two lines. One short white subline. White pill CTA. Shoe at a dynamic angle on wet asphalt with an orange rim light. |

**Rules**
- One family. Hierarchy from **weight** (Black/Bold vs Regular), **case** (ALL CAPS headline), **width** (condensed), **tracking** (tight on big, normal on small).
- Headline = verb + benefit ("RUN FURTHER") not category ("Running Shoes").
- Max 3 sizes. Leading on big headlines ~0.9.

**Prompt language**
```text
Typography-led design using ONE typeface family: a heavy condensed italic grotesk.
Headline "RUN FURTHER" in all caps, black weight, tight letter-spacing, line-height 0.9,
two lines, left-aligned, ~30% of canvas height. Subline "High performance shoes for
everyday runners." in regular weight, 1/6 of the headline size. No other fonts.
```

---

## 4. Give your elements room to breathe (Spacing)

**Crowding every corner feels messy. Spacing everything equally feels disconnected.**
Group related elements together, create enough space between sections.

| Before | After |
|---|---|
| Headline, subline, paragraph, two buttons all with the same gaps, product jammed underneath. | Title & tagline grouped tightly; paragraph separated; buttons grouped with a clear gap above; product given its own zone with air around it. Feels calm and premium. |

**Rules**
- **Proximity = relationship.** Small gaps inside a group, large gaps between groups (ratio ~1 : 3).
- Outer margins ~6–8% of width on all sides.
- 30–50% calm/empty space. Premium = more space.
- Align everything to one left edge (or one centre line) — never mixed.

**Prompt language**
```text
Generous whitespace and clear grouping. Outer margins of about 7% on all sides.
Headline and tagline sit tightly together as one group; the description is separated
by a larger gap; the two buttons form a third group below. All text left-aligned to the
same margin. The product sits in its own zone in the lower half with empty space
around it. About 40% of the canvas is calm empty background.
```

---

## 5. Break the pattern with intention (Variation)

**Perfectly aligned layouts and repeated elements feel predictable.** Introduce an
unexpected crop, an oversized element, an asymmetric layout, or a different image scale.

| Before | After |
|---|---|
| Small can standing upright in the centre-right, title left, everything boxed and polite. | Can is GIANT, tilted diagonally, dripping with condensation, cropped by the right edge. "FUEL YOUR DAY" in heavy italic caps on the left on a deep blue gradient. |

**Rules**
- Exactly ONE break: oversize · crop off-frame · tilt/diagonal · asymmetry · overlap text.
- The break should *point at* or *frame* the headline, not fight it.
- Keep everything else disciplined so the break reads as intentional.

**Prompt language**
```text
Dynamic asymmetric layout. The can is oversized — taller than the canvas — tilted
~20° to the right, covered in cold condensation droplets, cropped by the right and
bottom edges. Headline "FUEL YOUR DAY" on the left third in heavy italic caps.
Background: deep blue (#0B2A6F) to lighter blue radial gradient behind the can.
```

---

## 6. Give people something to look at (Visuals)

**Too much plain text can make a design feel lifeless.** Use a relevant image, a close-up
crop, a graphic element, or a visual metaphor that supports your message.

| Before | After |
|---|---|
| White card, "Jeans" title, paragraph, folded jeans stack. Text-heavy, visually plain. | Low-angle portrait of a young man in a denim jacket against a blue sky, looking off-frame. "Timeless *Style*" — mixing upright and italic — over the sky. Emotion sells. |

**Rules**
- Sell the *feeling*: a person using/wearing the product beats a product on white.
- Close-up crops and low angles add drama.
- Text goes over the *calm* part of the image (sky, wall, shadow).
- Real photography style for people: natural skin texture, real light, a lens and angle.

**Prompt language**
```text
Lifestyle photograph as the hero: a young man in a classic denim jacket, shot from a
low angle with an 85mm lens, looking off-frame to the upper left, against a clear soft
blue sky. Natural skin texture with visible pores, no retouched plastic look, late
afternoon sunlight from the left. Headline "Timeless Style" over the empty sky area on
the left: "Timeless" in bold upright sans, "Style" in bold italic of the same family.
```

---

## The one-line summary

> Pick ONE hero, make it BIG, make everything else SMALL and QUIET, group things,
> leave space, add ONE surprise, and quote every word.
