# Bench-TooolKit

A small set of tools for everyday cell culture work. Pure HTML/JS, no install required: open in a browser and use it, on desktop or phone.

Live site: https://uldekeulden.github.io/Bench-TooolKit/

## Tools

### [Cell Count + Passage Calculator](https://uldekeulden.github.io/Bench-TooolKit/cell_count_passage_calculator.html)

Calculates cell concentration, total yield, count-based seeding, and confluency-based passage ratios. Works on both desktop and phone.

- Hemocytometer count to concentration, with dilution correction by sample:diluent ratio or by a direct factor
- Count-based seeding: suspension volume per vessel, total suspension, fresh medium to top up
- Confluency-based passaging: fraction of the current culture per target vessel, equivalent split ratio, implied starting confluency
- Growth rate back-calculation: average 24 h growth multiplier and doubling time from a real passage
- Culture-vessel area reference (dishes, plates, flasks, ibidi chamber)
- Cell numbers can be displayed as `1,234,567`, `1.23×10⁶`, or `1.23e6`, switchable from the top bar and remembered between sessions
- Volumes switch from µL to mL automatically above 2000 µL, including the unit labels and the status text
- Inputs accept exponential entry (`5e6`), with a live echo below the field to confirm the order of magnitude

### [Multi-Plate Planner](https://uldekeulden.github.io/Bench-TooolKit/multi_plate_planner.html)

Plan and track layouts across multiple plates/conditions in one place, with local save support.

## Usage

Just open the live link above. No sign-up, no server needed, and it works offline after the first load once fonts are cached.

On iPhone: open the link in Safari, tap the Share button, then "Add to Home Screen" to launch it like an app.

## Local setup

Clone the repo and open the `.html` files directly in a browser. No backend required.

```
git clone https://github.com/uldekeulden/Bench-TooolKit.git
cd Bench-TooolKit
open index.html   # macOS
# or just double-click index.html
```

## Icons

In `icons/`: `home-*` (toolbox), `calc-*` (calculator), `plate-*` (6-well plate), each at 32 / 180 / 192 / 512 px.

## Tech notes

- Pure frontend (HTML + CSS + JavaScript), no framework dependencies
- Data is stored locally in the browser (localStorage), never uploaded anywhere
- Font: [Rubik](https://fonts.google.com/specimen/Rubik) (Google Fonts)

## Acknowledgments

Built with help from [Claude](https://claude.ai) (Anthropic), which turned the bench-side ideas behind these tools into working code and helped iterate on the calculation logic, formatting behavior, and responsive layout.

The visual style of this project draws on [getdesign.md's design analysis of Sentry](https://getdesign.md/sentry/design-md) (dark dashboard, data-dense layout, pink-purple accent), adapted for a lab-bench tool context.

Thanks to the [VoltAgent](https://github.com/VoltAgent) team for maintaining [awesome-design-md](https://github.com/VoltAgent/awesome-design-md), which curates this design-reference system for AI coding agents.

getdesign.md notes that its content is an independent analysis of publicly observable design patterns, meant as a starting point for inspiration, and is not affiliated with or endorsed by Sentry. This reference is included here purely as a design-credit note.

## Disclaimer

These tools are bench planning aids for research use. Confluency-to-cell-number relationships vary by cell line, vessel, coating, and handling, so results are estimates and not a substitute for cell-line-specific SOPs or empirical growth curves.

## License

MIT
