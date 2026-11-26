# Power Electronics & PCB Design Portfolio

**Hardware Engineering Projects | Karachi Shipyard & Engineering Works (KSEW)**

![KiCad](https://img.shields.io/badge/EDA-KiCad-314CB0?style=flat-square&logo=kicad&logoColor=white)
![Hardware](https://img.shields.io/badge/Domain-Power%20Electronics-007ACC?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

This repository contains schematic capture, PCB layout, and 3D mechanical render files for two custom power electronics boards developed at **Karachi Shipyard & Engineering Works (KSEW)**.

## Repository Structure

```text
AC to DC Conveter/
├── docs/
│   ├── 3D_back.png
│   ├── 3D_front.png
│   ├── Routing.png
│   └── Schematic.png
└── AC_DC_converter.*

Power Supply/
├── docs/
│   ├── back.jpg
│   ├── Front.jpg
│   └── side.jpg
└── transformerlesspowersupply.*

.gitignore
LICENSE
README.md
```

## 12 V AC-to-DC Bridge Rectifier Converter

A compact, single-layer, through-hole full-wave bridge rectifier and capacitive filter module designed to convert a 12 V AC input into a smoothed DC output with visual power indication and bleeder discharge protection.

### Bill of Materials

| Reference | Component | Value or part number | Role |
| --- | --- | --- | --- |
| J1, J2 | Screw terminals | `Screw_Terminal_01x02` | 12 V AC input and filtered DC output |
| D1-D4 | Rectifier diodes | `1N4007` (×4) | Full-wave bridge rectification |
| C1 | Electrolytic capacitor | `1000 µF` | Output ripple filtering and DC smoothing |
| R1 | Current-limiting resistor | `2.2 kΩ` | Limits current through the indicator LED |
| R2 | Bleeder resistor | `10 kΩ` | Discharges C1 when power is removed |
| D5 | Indicator LED | Standard LED | Indicates DC output power |

### Schematic and PCB Preview

| Schematic | PCB Routing |
| --- | --- |
| ![Schematic](<AC to DC Conveter/docs/Schematic.png>) | ![PCB routing](<AC to DC Conveter/docs/Routing.png>) |

| 3D Front View | 3D Back View |
| --- | --- |
| ![3D front view](<AC to DC Conveter/docs/3D_front.png>) | ![3D back view](<AC to DC Conveter/docs/3D_back.png>) |

## Transformerless Regulated Power Supply

A compact capacitive-dropper regulated DC power supply PCB for low-power auxiliary and control electronics, without the footprint or weight of a step-down transformer.

### Design Highlights

- **Capacitive dropper:** High-voltage X2 film capacitor paired with series surge-limiting and discharge resistors.
- **Rectification and filtering:** Discrete rectifier stage with dual electrolytic smoothing capacitors.
- **Linear voltage regulation:** TO-220 package regulator providing a stable DC rail to the output screw terminal block.
- **Status indication:** On-board power indicator LED and 2-pin screw terminals for AC mains input and regulated DC output.

> [!WARNING]
> Transformerless power supplies are **not galvanically isolated** from the AC mains. Keep the board inside a fully insulated enclosure and avoid touching conductive traces or components while energized.

### Mechanical Previews

| Top / Front View | Bottom / Solder Side | Side Profile |
| --- | --- | --- |
| ![Top and front view](<Power Supply/docs/Front.jpg>) | ![Bottom view](<Power Supply/docs/back.jpg>) | ![Side profile](<Power Supply/docs/side.jpg>) |

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/imeesam/karachi-shipyard-power-electronics.git
   cd karachi-shipyard-power-electronics
   ```

2. Open a project in KiCad:

   - Open `AC_DC_converter.kicad_pro` in `AC to DC Conveter/`.
   - Open `transformerlesspowersupply.kicad_pro` in `Power Supply/`.

3. Inspect or manufacture:

   - View schematics in the Schematic Editor.
   - Inspect track widths and clearances in the PCB Editor.
   - Export Gerber and drill files for fabrication.

## KiCad

The projects were created with KiCad. KiCad 6.0 or later is recommended.

## Author

**Meesam**

Power Electronics & PCB Design - Karachi Shipyard & Engineering Works (KSEW)

## License

See [LICENSE](LICENSE) for license terms.
