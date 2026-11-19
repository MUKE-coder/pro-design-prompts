# Template: Infographic / Data Post

One insight per image. Numbers are the hero. **Check every number afterwards.**

## Design Decisions
```text
FORMAT:     [4:5]
HERO:       the key number "[73%]" at ~25% of canvas height
HIERARCHY:  1 [big number] → 2 [what it means, 1 line] → 3 [2–4 supporting items] → 4 [source]
LAYOUT:     big number top-left; supporting items as a simple [vertical list / 2×2 grid / bar row]
TYPE:       one sans family; number in black weight; labels regular
COLOUR:     neutral bg [#F5F7FA], ONE accent [#1F4BFF] used only for the highlighted data
BREAK:      the number is so big it's cropped slightly by the left edge
SPACE:      45%
NO:         3D charts, pie charts with many slices, icons for every line, gradients, clip-art people
```

## Prompt
*(The numbers below are placeholders, not real data — replace with your sourced figures.)*
```text
Create a flat 2D infographic social post, 4:5 portrait, edge-to-edge, editorial data
design style like a Financial Times / Bloomberg graphic. Background plain [#F5F7FA].

TEXT and DATA — render exactly, no other text or numbers anywhere:
- Top-left, enormous black-weight sans-serif in [#1F4BFF]: "[73%]"
- Directly under, medium bold near-black, 2 lines: "[of Kampala SMEs now take mobile money]"
- Middle: a simple horizontal bar chart with [3] flat bars, labels left, values right:
  "[2022]" "[41%]" · "[2024]" "[58%]" · "[2026]" "[73%]" — only the last bar in [#1F4BFF],
  others light grey [#D5DAE1]. Bar lengths proportional to the values.
- Bottom-left, tiny grey: "Source: [SOURCE NAME, YEAR]"
- Bottom-right, tiny: "[@handle]"

LAYOUT: 8% margins, left-aligned, generous spacing, 45% empty.
DO NOT INCLUDE: 3D, shadows, gradients, icons, people, extra numbers, extra text, decoration.
```

> Numbers in charts are often drawn wrong by image models. For anything with real data,
> make the chart in Canva/Figma/Sheets and use the image model only for the visual style.
