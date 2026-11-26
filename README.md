Here is a clean, ready-to-paste `README.md` tailored to your exact folder structure, KiCad files, image paths, and Karachi Shipyard & Engineering Works (KSEW) experience.

Copy the Markdown below directly into your root `README.md` file:

```markdown
# Power Electronics & PCB Design Portfolio
**Hardware Engineering Projects | Karachi Shipyard & Engineering Works (KSEW)**

![KiCad](https://img.shields.io/badge/EDA-KiCad-314CB0?style=flat-square&logo=kicad&logoColor=white)
![Hardware](https://img.shields.io/badge/Domain-Power%20Electronics-007ACC?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

This repository contains complete schematic capture, PCB layout, and 3D mechanical render files for two custom power electronics boards designed during my experience at **Karachi Shipyard & Engineering Works (KSEW)**.

---

## Repository Structure

```text
├── AC to DC Conveter/
│   ├── docs/
│   │   ├── 3D_back.png
│   │   ├── 3D_front.png
│   │   ├── Routing.png
│   │   └── Schematic.png
│   └── AC_DC_converter.*        # KiCad project, schematic, and PCB layout files
│
├── Power Supply/
│   ├── docs/
│   │   ├── back.jpg
│   │   ├── Front.jpg
│   │   └── side.jpg
│   └── transformerlesspower.*   # KiCad project, schematic, and PCB layout files
│
├── .gitignore
├── LICENSE
└── README.md

```

---

## 1. 12V AC-to-DC Bridge Rectifier Converter

A compact, single-layer through-hole full-wave bridge rectifier and capacitive filter module designed to convert a 12V AC input into a smoothed DC output with visual power indication and bleeder discharge protection.

### Key Specifications & Bill of Materials (BOM)

| Reference | Component | Value / Part Number | Role |
| --- | --- | --- | --- |
| **J1, J2** | Screw Terminals | `Screw_Terminal_01x02` | 12V AC Input (`J1`) & Filtered DC Output (`J2`) |
| **D1 – D4** | Rectifier Diodes | `1N4007` (×4) | Full-wave bridge rectification |
| **C1** | Electrolytic Capacitor | `1000 µF` | Output ripple filtering & DC smoothing |
| **R1** | Current-Limiting Resistor | `2.2 kΩ` | Limits current through the indicator LED |
| **R2** | Bleeder Resistor | `10 kΩ` | Safely discharges `C1` when power is removed |
| **D5** | Indicator LED | Standard LED | Visual DC output power indicator |

### Design & 3D Previews

| Schematic | PCB Routing |
| --- | --- |
|  |  |

| 3D Front View | 3D Back View |
| --- | --- |
|  |  |

---

## 2. Transformerless Regulated Power Supply

A compact capacitive-dropper regulated DC power supply PCB engineered for low-power auxiliary and control electronics without the footprint or weight of a step-down transformer.

### Design Highlights

* **Capacitive Dropper Stage:** High-voltage X2 film capacitor paired with series surge-limiting and discharge resistors.
* **Rectification & Filtering:** Discrete rectifier diode stage with dual electrolytic smoothing capacitors.
* **Linear Voltage Regulation:** TO-220 package linear voltage regulator providing a stable, regulated DC rail to the output screw terminal block.
* **Status Indication:** On-board power indicator LED and 2-pin screw terminals for AC mains input and regulated DC output.

> **Safety Note:** Transformerless power supplies are **not galvanically isolated** from the AC mains. Keep the board inside a fully insulated enclosure and avoid touching any conductive traces or components while energized.

### 3D Mechanical Previews

| Top / Front View | Bottom / Solder Side | Side Profile |
| --- | --- | --- |
|  |  |  |

---

## Getting Started

1. **Clone the repository:**
```bash
git clone [https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git](https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git)

```


2. **Open in KiCad:**
* Launch **KiCad** (v6.0 or later recommended).
* Open `AC_DC_converter.kicad_pro` inside `AC to DC Conveter/` or `transformerlesspower.kicad_pro` inside `Power Supply/`.


3. **Inspect or Manufacture:**
* View schematics in the **Schematic Editor**, inspect track widths and clearances in the **PCB Editor**, or export Gerber/Drill files for fabrication.



---

## Author

**Meesam**

Power Electronics & PCB Design — Karachi Shipyard & Engineering Works (KSEW)

```

### Quick Tip Before You Push
* Notice your folder is currently named `AC to DC Conveter` (missing the `r` in *Converter*)—the image links in the `README.md` above already match that exact folder name (`AC%20to%20DC%20Conveter`) so all your pictures will render properly on GitHub right away.
* Replace `YOUR-USERNAME/YOUR-REPO-NAME` in the `git clone` command with your actual GitHub username and repository name once you create it.

```