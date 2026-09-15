# Bench-TooolKit

A small set of tools for everyday cell culture work. Pure HTML/JS, no install required — open in a browser and use it, on desktop or phone.

Live site: **https://uldekeulden.github.io/Bench-TooolKit/**

## Tools

### <img src="icons/calc-32.png" width="20"> [Cell Count + Passage Calculator](https://uldekeulden.github.io/Bench-TooolKit/cell_count_passage_calculator.html)
Calculates cell concentration, total yield, count-based seeding, and confluency-based passage ratios. Works on both desktop and phone.

### <img src="icons/plate-32.png" width="20"> [Multi-Plate Planner](https://uldekeulden.github.io/Bench-TooolKit/multi_plate_planner.html)
Plan and track layouts across multiple plates/conditions in one place, with local save support.

## Usage

Just open the live link above — no sign-up, no server needed (works offline after the first load, once fonts are cached).

On iPhone: open the link in Safari → tap the Share button → "Add to Home Screen" to launch it like an app.

## Local setup

Clone the repo and open the `.html` files directly in a browser — no backend required.

```bash
git clone https://github.com/uldekeulden/Bench-TooolKit.git
cd Bench-TooolKit
open index.html   # macOS
# or just double-click index.html
```

## Icons

In `icons/`: `home-*` (toolbox), `calc-*` (calculator),
`plate-*` (6-well plate), each at 32 / 180 / 192 / 512 px.

## Tech notes

- Pure frontend (HTML + CSS + JavaScript), no framework dependencies
- Data is stored locally in the browser (localStorage), never uploaded anywhere
- Font: [Rubik](https://fonts.google.com/specimen/Rubik) (Google Fonts)

## Acknowledgments

The visual style of this project draws on [getdesign.md's design analysis of Sentry](https://getdesign.md/sentry/design-md)
(dark dashboard, data-dense layout, pink-purple accent), adapted for a lab-bench tool context.

Thanks to the [VoltAgent](https://github.com/VoltAgent) team for maintaining
[awesome-design-md](https://github.com/VoltAgent/awesome-design-md), which curates this
design-reference system for AI coding agents.

> getdesign.md notes that its content is an independent analysis of publicly observable design
> patterns, meant as a starting point for inspiration, and is not affiliated with or endorsed by
> Sentry. This reference is included here purely as a design-credit note.

## License

MIT
