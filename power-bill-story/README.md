# Who Pays for the Cloud

An illustrated scroll story about rising household electricity bills, the data center boom, and how costs reach homes. It ends with a petition.

The whole story happens in one 3D town. The camera moves through the town as you scroll, and the town changes with the story. A utility-bill stub stays on screen and moves forward in time from 2020 to 2026.

| Chapter | Scene |
| --- | --- |
| Hero | The town at night, seen from above. |
| 01 Your home | The camera moves down to one house. The bill shows $119 (2020). |
| 02 The grid | Power pulses move from the plant, through the transmission lines and the substation, to the streets. |
| 03 A new neighbor | A crane appears and a data center campus rises. A new line connects it to the town substation. |
| 04 A crowded grid | Cyan pulses take more of the power. PJM capacity prices are shown as a bar chart. |
| 05 The build-out | A new high-voltage line and a new substation are built. Red cost pulses move from them to every house. |
| 06 Back home | The same house. The bill is now $169. A line chart shows the change. |
| 07 A fairer deal | Solar panels and batteries appear. The cost pulses go to the data center, not to the houses. |
| 08 Take action | Dawn comes over the town. The petition form. When someone signs, a wave of light moves across the houses. |

Colour has one meaning everywhere: amber is power to homes, cyan is power to data centers, coral is cost, and mint is on-site clean power.

## How it is built

- **Anime.js 4**: one `createTimeline()` linked to scroll with `onScroll({ sync })`. It controls the camera path, the year on the bill, every building that grows in, the flow amounts, the 3D tags, and the charts (`svg.createDrawable` draws the line). Each story card also has its own scroll-linked entrance.
- **Three.js**: the town is procedural. It uses instanced houses, trees and windows, lattice pylons with sagging wires, a hyperboloid cooling tower with steam, wind turbines, and a data center with spinning rooftop fans. Unreal bloom makes the lights glow.

## Data

The bill uses 900 kWh a month at the U.S. average residential price from the EIA (13.2¢ in 2020, 18.8¢ in April 2026). The page footer lists all sources. The town is an illustration, not a real place.

## Petition

The form is a front-end prototype. It checks the fields and shows a thank-you state. It does not send data. Connect it to your advocacy platform before you launch it.

## Run it

```sh
npx serve power-bill-story
```
