# Worked Examples: Slop Prompt → Pro Prompt

Each example shows the prompt people usually write, what goes wrong, and the rewrite.
Brands are fictional — swap in your own (and upload your real logo/product).

---

## 1. Sale ad (Hierarchy)

**❌ Slop prompt**
> Make a modern, eye-catching sale poster for my online store, 70% off, colourful and stunning.

*Result:* rainbow gradient, sparkles, 4 fonts, "70% OFF" same size as 3 other lines, random shopping bags floating.

**✅ Pro prompt**
```text
Flat 2D social media sale ad, 4:5, edge-to-edge, not a mockup.
Background: saturated orange gradient from #FF7A00 (top) to #E63E00 (bottom).
Hero: three plain kraft-paper shipping boxes, stacked, large, cropped by the right edge,
soft studio light from upper left, realistic cardboard texture.
Text — exactly as written, no other text:
- Top-left, white, extra-bold neo-grotesk sans, 3 stacked lines, ~13% of height each:
  "Mega" / "Weekend" / "Sale"
- Below, a bright yellow #FFD400 rectangle tilted −4° containing black text: "Up to" (small)
  and "70% Off" (twice as large, black weight)
- Small white regular text below: "Electronics, fashion, home and more."
- White pill button with dark text: "Shop Now →"
7% margins, left-aligned, headline is the dominant element, 30% calm space.
Do not include: sparkles, confetti, shopping bags, people, extra text, drop shadows, purple.
```

---

## 2. Fast-food (Contrast)

**❌** "A delicious chicken burger ad, appetizing, high quality, 8k."

*Result:* beige background, centred burger with steam, tiny grey title. Flat.

**✅**
```text
Flat 2D fast-food ad, 4:5. Solid deep red #C8102E background; one oversized golden curved
shape bleeding off the top-right corner. Two-tone headline top-left in one extra-bold rounded
sans: "Chicken" white, "Burger" golden yellow #FFC72C, two lines, very large.
Small white subline: "A classic favourite for any time of the day."
Hero: crispy chicken burger, sesame bun, lettuce, creamy sauce, front three-quarter view,
warm 45° side light, real texture, large, lower right, cropped by the bottom edge.
No steam, no smoke, no fries, no drinks, no extra text, no drop shadows.
```

---

## 3. Running shoe (Typography)

**❌** "Nice ad for running shoes with text 'Running Shoes, high performance, shop now', modern font."

**✅**
```text
Flat 2D sportswear ad, 4:5. Dark charcoal #121212 background with one diagonal streak of
orange #FF5A1F light from the lower right. Hero: a white-and-black running shoe (unbranded)
at a dynamic low angle on wet dark asphalt, orange rim light, lower half, slightly tilted.
Typography: ONE heavy condensed italic grotesk. Headline top-left, white, all caps, tight
tracking, line-height 0.9: "RUN" / "FURTHER", ~30% of canvas height combined.
Subline small regular white: "High performance shoes for everyday runners."
White pill button: "Shop Now →". No other fonts, no other text.
```

---

## 4. Phone launch (Spacing)

**❌** "iPhone-style ad with title, tagline, description, two buttons and phone image."

*Result:* everything crammed, equal gaps, phone touching text.

**✅**
```text
Flat 2D tech product page hero, 4:5, off-white #F5F5F7 background, premium minimal product
page art direction. Group 1 (tight): headline "Nova 5" in bold near-black neo-grotesk,
very large, with tagline "Built for what's next." directly below in medium weight.
Larger gap. Group 2: description "A powerful chip, a better camera, and longer battery
life." small regular grey #6E6E73. Larger gap. Group 3: two buttons side by side — black
pill "Learn More →" and outlined pill "Buy Now". Lower 45%: the back of a lavender
smartphone with a dual camera, cropped by the bottom and right edges, soft top light.
All text left-aligned at 8% margin. 40% empty space. No other text.
```

---

## 5. Energy drink (Break the pattern)

**❌** "Energy drink can on blue background with text Energy Drink."

**✅** see `models/gpt-image.md` — oversized can, 20° tilt, cropped off-frame, condensation,
"FUEL / YOUR / DAY" heavy italic caps on the left.

---

## 6. Denim brand (Visuals)

**❌** "Jeans ad, folded jeans, text 'Our Jeans, timeless and comfortable'."

**✅**
```text
Flat 2D fashion ad, 4:5. Full-bleed lifestyle photograph: a young man in a classic
mid-blue denim jacket over a white T-shirt, low angle, 85mm, looking off-frame to the upper
left, against a clear soft blue sky; late-afternoon sun from the left; natural skin texture
with visible pores, realistic fabric. Subject occupies the right 60%.
Over the empty sky on the left: "Timeless" in bold upright white sans and "Style" in bold
italic white of the same family, stacked, large. Small white subline: "Everyday comfort
that never goes out of style." White pill "Shop Now →". No other text, no logos.
```

---

## 7. Gospel concert flyer (local example)

**❌** "Church crusade poster, Jesus, light, doves, worship, Sunday 6pm Kampala, colourful."

*Result:* clip-art doves, rays, 5 fonts, misspelled venue, invented phone number.

**✅** see `templates/event-flyer.md` and `models/ideogram-flux-others.md` (A Night of Worship).
