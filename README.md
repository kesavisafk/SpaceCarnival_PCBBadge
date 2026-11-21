# TinkerSpace PCB Badge 2026 — Space Carnival Competition Entry

A PCB badge design submitted as an entry for the **Space Carnival 2026 PCB Badge Competition**. This repository contains the fabrication files for the badge, along with space to document the design and its development.


## Design

The physical layout of the badge combines a heart with a gear, representing my love for maker culture — the passion for creating, experimenting, building things, and learning by making. The design brings together the heart behind creativity and the mechanical side of making, with TinkerSpace's signature blue and yellow as its primary colours.

The circuit uses a 555 timer, a timing capacitor, resistors, and LEDs to create a flashing pattern of alternating yellow and blue lights. The board is powered by 5V through a USB-C connector.

But the main idea behind the badge goes beyond simply lighting up. I wanted the badge to encourage interaction and collaboration, making the PCB itself a part of the experience. Exposed contact pads on the top of the board allow two badges to be brought together and touched against each other. The LEDs only light up when two boards make contact, turning a standalone badge into something that comes alive through interaction.

The idea is to make the badge more than something you wear — it's something you can connect with someone else, quite literally. A small reminder that maker culture is built around sharing ideas, collaborating, and creating things together.

### Preview



| Front view | Back view |
| --- | --- |
| [Front view](docs/images/front.png) | [Back view](docs/images/back.png) |

*The LEDs appear red in the preview images. The actual badge will use alternating yellow and blue LEDs, switching between each other as the circuit cycles between HIGH and LOW states.*


## Bill of materials

The complete component list is also available in [`Tinkerspace PCB.csv`](Tinkerspace%20PCB.csv). The table below summarises the parts used on one badge. Prices are indicative unit estimates based on bulk sourcing at approximately 300 pieces; actual supplier quotations may vary and may exclude GST, shipping, and minimum-order charges.

| Designator | Qty. per badge | Component | Package / value | Estimated unit price | Estimated line total | Source |
| --- | ---: | --- | --- | ---: | ---: | --- |
| R1, R2, R3, R5–R9 | 8 | Resistors | 0805; 1 kΩ, 5.1 kΩ, 150 Ω, 330 kΩ | ₹0.06 | ₹0.48 | [Adinath Electronics – 0805 SMD resistors](https://www.adinathelectronics.com/sitemap.html) |
| R4 | 1 | Resistor | Axial, 1 kΩ | ₹0.50 (assumed) | ₹0.50 | Local electronics suppliers |
| D1–D4 | 4 | Yellow LEDs | 3 mm through-hole | ₹0.40 | ₹1.60 | [Adinath Electronics – 3 mm yellow LED](https://www.adinathelectronics.com/sitemap.html) |
| D5–D8 | 4 | Blue LEDs | 3 mm through-hole | ₹0.40 | ₹1.60 | [Adinath Electronics – 3 mm blue LED](https://www.adinathelectronics.com/sitemap.html) |
| U1 | 1 | NE555P timer IC | DIP-8 | ₹4.00–₹7.00 (estimated) | ₹4.00–₹7.00 | Electronics component suppliers (bulk estimate) |
| Q1 | 1 | BC557 PNP transistor | TO-92 | ₹2.24 | ₹2.24 | [Sunrom Electronics](https://www.sunrom.com/) |
| C1 | 1 | Timing capacitor | 1 µF, radial | ₹0.50 (assumed) | ₹0.50 | Local electronics suppliers |
| J1 | 1 | USB-C receptacle | GCT USB4125 series, 6-pin | ₹7.00 (estimated) | ₹7.00 | [GCT](https://gct.co/) / electronics distributors |
| TP1, TP2 | 2 | Contact / test pads | PCB pads | Included in PCB fabrication | — | Part of the PCB copper layout |

**Estimated component cost per badge: ₹17.92–₹20.92.**  
**Estimated PCB fabrication cost per badge: ₹23.00–₹28.00.**  
**Estimated total per badge, including PCB fabrication: ₹40.92–₹48.92** (excluding assembly, GST, and shipping).

The ₹0.50 unit prices for the axial resistor and timing capacitor are assumptions for a bulk order of around 300 pieces. The USB-C receptacle is estimated at ₹7.00 per unit, and the NE555P timer IC is estimated at ₹4.00–₹7.00 per unit. PCB fabrication is estimated at ₹23.00–₹28.00 per board. Other component prices are indicative bulk unit prices and should be confirmed with suppliers before procurement. These figures are per-badge estimates, not the total cost of producing 300 badges.

## Fabrication files

The `SpaceCarnival_PCBBadge` folder contains the Gerber and drill files exported for PCB fabrication.

| File | Layer / purpose |
| --- | --- |
| `Tinkerspace PCB-F_Cu.gbr` | Front copper |
| `Tinkerspace PCB-B_Cu.gbr` | Back copper |
| `Tinkerspace PCB-F_Mask.gbr` | Front solder mask |
| `Tinkerspace PCB-B_Mask.gbr` | Back solder mask |
| `Tinkerspace PCB-F_Silkscreen.gbr` | Front silkscreen |
| `Tinkerspace PCB-B_Silkscreen.gbr` | Back silkscreen |
| `Tinkerspace PCB-F_Paste.gbr` | Front paste |
| `Tinkerspace PCB-B_Paste.gbr` | Back paste |
| `Tinkerspace PCB-Edge_Cuts.gbr` | Board outline |
| `Tinkerspace PCB-PTH.drl` | Plated through-hole drill data |
| `Tinkerspace PCB-NPTH.drl` | Non-plated through-hole drill data |
| `Tinkerspace PCB-job.gbrjob` | Gerber job file |

## PCB layout



| Front layout | Back layout |
| --- | --- |
| [Front layout](docs/images/front-layout.png) | [Back layout](docs/images/back-layout.png) |


## Submission notes

This project is a competition entry for Space Carnival 2026. The files and images in this repository are intended to present the badge design and provide the PCB fabrication data for review.

