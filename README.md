# usb-to-uart-cp2102n
KiCad project: USB to UART converter based on CP2102N
This is a simple USB to UART converter board designed in **KiCad**, built around the **CP2102N** USB-to-Serial bridge IC.

## ✏️ About
This project converts USB signals to standard UART (TX, RX) levels, making it easy to interface a computer to microcontrollers, sensors, and other serial devices.  

It includes:
- CP2102N USB-to-UART IC
- USB connector (e.g., USB-C)
- Status LEDs (TX/RX)
- Filter capacitors
- UART header pins (TX, RX, , RST, GND, etc.)

## 📂 Project structure
- `USB TO UART.kicad_sch` – Schematic file
- `usb-to-uart.kicad_pcb` – PCB layout file
- `usb-to-uart.kicad_pro` – KiCad project file
- `symbols/` – Custom schematic symbols 
- `footprints/` – Custom footprints
- `gerber/` – Gerber and drill files for fabrication
- `bom.csv` – Bill of Materials

- ## ⚙️ Tools
- Designed with [KiCad](https://kicad.org/)

- ## 📦 Fabrication
Use the files in the `gerber/` directory to order PCBs from manufacturers (e.g., JLCPCB etc.).

## 💡 Features
- CP2102N supports full-speed USB 2.0
- The CP2102N receives power from USB VBUS (5 V), connected to the REGIN pin. Its internal 3.3 V regulator outputs on VDD, with a 100 nF decoupling capacitor. This VDD rail powers the chip and defines the logic level for all UART signals (TX, RX, etc). Therefore, the UART interface operates at standard 3.3 V logic levels.
- Status LEDs for data transmission/reception
- Compact 2-layer PCB

- ## 📄 License
MIT License – feel free to modify and use.

## 🙌 Contributions
Pull requests welcome! If you spot issues or have improvements, please open an issue or PR.
