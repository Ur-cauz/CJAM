<div align="center">

# CJAM

### Open-Source ESP32 + Triple NRF24L01+ Development Board

*A compact ESP32 development board designed for 2.4 GHz experimentation, embedded development, RF learning, and wireless security research.*

![Status](https://img.shields.io/badge/Status-Prototype%20Ordered-blue?style=for-the-badge)
![Open Source](https://img.shields.io/badge/Open-Source-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Designed With](https://img.shields.io/badge/Designed%20With-EasyEDA-orange?style=for-the-badge)

</div>

---

# About

CJAM began because I got tired of rebuilding the same project repeatedly.

Originally, this setup was on a breadboard before I soldered it onto a prototype board. While it worked, it wasn't visually appealing—I spent hours soldering wires, correcting mistakes, and burning my fingers more times than I care to admit, only to end up with something I didn't like.

Instead of going through that process every time I wanted to experiment, I decided to create a proper PCB.

CJAM combines an ESP32, three NRF24L01+ modules, an OLED display, dedicated power filtering, a user button, and a status LED into one compact board that's easy to assemble, reuse, and expand.

I also aimed to document everything and make it open source. I want anyone interested in electronics, PCB design, embedded systems, RF, or hardware security research to learn from it, improve it, or build their own.

---
# >**< Showcase

| PCB Front | PCB Back |
|------------|----------|
| <img src="/Images/pcb-front.png" width="450"> | <img src="/Images/pcb-back.png" width="450"> |

| PCB Routing | 3D Case |
|-------------|-----------|
| <img src="/Images/pcb-routing.png" width="450"> | <img src="/Images/case-render.png" width="450"> |

| Schematic |
|----------|
| <img src="/Images/schematic.png" width="450"> |
# Features
 
- ESP32 DevKit V1 (38-Pin)
- Support for **3× NRF24L01+ Modules**
- Dedicated **100µF + 0.1µF** decoupling capacitors for each NRF24L01
- 0.96" I²C OLED Display
- User Push Button
- Status LED
- Clearly labeled GPIO headers
- 2-Layer PCB
- Designed in EasyEDA
- Optional 3D Printable Enclosure
- Open Source Hardware
- Firmware examples included

---

# Applications

CJAM serves as a general-purpose 2.4 GHz experimentation platform.

Some possible uses include:

- Learning Embedded Systems
- Learning SPI Communication
- Learning RF Fundamentals
- NRF24L01 Development
- ESP32 Development
- Wireless Communication Projects
- Rapid Hardware Prototyping
- Educational Projects
- 2.4 GHz Experimentation
- Authorized Wireless Security Research

---

# Hardware

## Components

| Qty | Component |
|----:|-----------|
| 1 | ESP32 DevKit V1 (38-Pin) |
| 3 | NRF24L01+ Modules |
| 3 | 100µF / 6.3V Electrolytic Capacitors |
| 3 | 0.1µF Ceramic Capacitors |
| 2 | 4.7kΩ Resistors |
| 1 | 1kΩ Resistor |
| 1 | Status LED |
| 1 | Tactile Push Button |
| 1 | 0.96" I²C OLED Display |

---

# GPIO Mapping

| ESP32 GPIO | Function |
|------------|----------|
| GPIO21 | OLED SDA |
| GPIO22 | OLED SCL |
| GPIO18 | Shared SPI SCK |
| GPIO19 | Shared SPI MISO |
| GPIO23 | Shared SPI MOSI |
| GPIO17 | NRF24 #1 CE |
| GPIO16 | NRF24 #2 CE |
| GPIO5 | NRF24 #3 CE |
| GPIO15 | NRF24 #1 CSN |
| GPIO4 | NRF24 #2 CSN |
| GPIO27 | NRF24 #3 CSN |
| GPIO2 | Status LED |
| GPIO13 | User Push Button |

---

# Repository Structure

```text
CJAM/
│
├── hardware/
│   ├── EasyEDA/
│   ├── Gerbers/
│   ├── Schematic/
│   ├── Datasheets/
│   └── Images/
│
├── firmware/
│   ├── Examples/
│   └── Source/
│
├── enclosure/
│   ├── STL/
│   └── STEP/
│
├── docs/
│   ├── Assembly.md
│   ├── Wiring.md
│   ├── Hardware.md
│   ├── Firmware.md
│   └── Revision-History.md
│
├── LICENSE
└── README.md
```

---

# Project Status

- ✅ Schematic Complete
- ✅ PCB Designed
- ✅ DRC Passed
- ✅ Prototype Ordered
- 🚧 Firmware Development
- ⏳ Prototype Validation
- ⏳ Documentation
- ⏳ Revision 2

---

# Open Source

Everything needed to build CJAM yourself is included in this repository.

Included files:

- EasyEDA Project
- Gerber Files
- Schematics
- Datasheets
- Firmware Examples
- Assembly Guide
- 3D Printable Enclosure
- Documentation

If you build one, improve it, or use it in another project, I would love to see it.

Pull requests, issues, and suggestions are always welcome.

---

# Credits

Thanks to:

- **EasyEDA Documentation** for helping me learn PCB design and understand the software.
- **Espressif's ESP32 Datasheets** for enabling me to create custom schematic symbols and footprints used throughout this project.

---

# Disclaimer

CJAM is an open-source hardware platform for education, embedded development, hardware experimentation, RF learning, and **authorized** wireless security research.

Always make sure you have permission before testing or interacting with networks or devices that you do not own or control.

You are solely responsible for following the laws and regulations that apply in your area.

The author takes no responsibility for misuse of this project.

---

# License

This project is licensed under the **MIT License**.

See the [LICENSE](LICENSE) file for details.

---

<div align="center">

### Made with too much coffee, burnt fingers, and way too many jumper wires.

**— Cauz**

If you found this project interesting, consider giving it a star!

</div>
