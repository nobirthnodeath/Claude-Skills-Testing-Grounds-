# Anatomy of a Wash

A scroll-scrubbed product teardown of the **LG WM4000HWA** front-load washer (4.5 cu ft, 1,300 rpm, Inverter Direct Drive).

Scroll down to move forward. Scroll up to move back.

| Phase | What happens |
| --- | --- |
| 01 Exterior | The white, colour-rendered machine turns a full 360°. |
| 02 X-ray | A scan plane moves down the machine. Above the plane, the enamel changes to a glowing wireframe. The studio background changes to a blueprint field. Lines for the overall dimensions draw in. |
| 03 Explode | 20 assemblies move apart along the drum axis, in teardown order. |
| 04 Anatomy | Numbered callouts draw one at a time. Each part flashes as its callout appears. Hover a callout to highlight its part. |
| 05 Spec | The drawing frame and the title block close the sheet. |

## How it is built

- **Anime.js 4** controls all motion. One `createTimeline()` is linked to the page scroll with `onScroll({ sync })`, so the scroll position sets the timeline position. The timeline tweens plain JS state (yaw, scan height, explode amount, camera), DOM (chapters, HUD colour via a CSS variable), and SVG (`svg.createDrawable` for the drawing frame). `stagger` sets the explode and callout order. `splitText` animates the hero title on load.
- **Three.js** draws the model. All geometry is procedural (lathe, extrude, tube, rounded box), with physical materials and a room environment map. The X-ray effect uses two opposed clipping planes: solid surfaces stay below the plane, and the wire and ghost layers show above it. A small line shader adds the hot edge at the scan plane and the amber highlight. Unreal bloom gives the glow.

The model is an interpretation based on LG front-load service documentation (cabinet, tub and drum exploded views). Proportions are approximate. This is an independent study and is not affiliated with LG Electronics.

## Run it

Open `index.html` through any static server, for example:

```sh
npx serve washing-machine-anatomy
```

The page loads Three.js and Anime.js from jsDelivr, so it needs a network connection. It honours `prefers-reduced-motion`: scroll still scrubs, but idle motion stops.
