# UI experiments: kitchen app

Visual exploration only. Features and tasks stay the same as the current app.

- `kitchen-directions.html`: round 1. Market Stall, Label Maker, Cold Storage.
- `kitchen-directions-round-2.html`: round 2, based on Market Stall. Fresh Picks, Sorbet, Evening Kitchen (warm dark).
- `reference/`: screenshots of the current app.

Each direction shows Home (quiet week), Home (9 expired), the sort screen, and Inventory. Open a file in a browser.

## Round 3

- `design-principles.md`: six ranked principles from the round 2 feedback (made with the `design-principles` skill).
- `prototype-home-inventory.html`: throwaway prototype (made with the `prototype` skill). Three layouts for Home and Inventory, each in light and warm dark. Switch with `#a`, `#b`, `#c`, the bottom bar, or the arrow keys.

## Round 4

- `prototype-themes.html`: the Calm list layout with a cook card (no button, right chevron) and no "Less than usual" tag. Three themes: light, cocoa dark, graphite dark. Switch with `#light`, `#cocoa`, `#graphite`, the bottom bar, or the arrow keys.
- `design-principles.md`: added the round 4 decision on cards and depth.

## Round 5

- `prototype-themes.html` updated: the expired alert is now a red-tinted card with "9 things expired" as text (no number circle). Graphite dark has no warm or brown tones.

## Round 6

- `prototype-themes.html` now shows only Light and Graphite, side by side, with full-length Home screens. No yellow. Green primary actions. Text-only cook card with a periwinkle tint. "Sort" text link on the expired card. Faint color fringes in the Graphite background.
- `design-principles.md`: principle 2 updated for green actions and no yellow.

## Round 7

- `prototype-dark-motion.html`: Graphite only, with a live WebGL background (three.js r128 from cdnjs and a custom shader). Three looks: Aurora, Lens, Prism (`#aurora`, `#lens`, `#prism`). The bottom bar has look, strength and pause controls. Motion stops if the viewer has asked for reduced motion.

## Round 8

- `prototype-mesh-gradient.html`: Graphite with a moving background from `@mesh-gradient/core` 2.0.2 (loaded from jsDelivr). An SVG filter adds the chromatic-aberration color split. Three palettes: Nightfall, Prism, Smoke (`#nightfall`, `#prism`, `#smoke`). The bottom bar has palette, color split, speed and pause controls.
