# ESP32-S3 Dual USB-C Development Board

This repository contains a complete Altium Designer hardware project for a custom ESP32-S3 Mini development board. The design focuses on robust USB connectivity, safe power handling, and standard layout techniques for microcontroller applications.

## Hardware Specifications & Features
* **Microcontroller:** ESP32-S3 Mini module.
* **Dual USB-C Interfaces:**
  * **Port 1 (UART):** Routed through an onboard FTDI USB-to-UART bridge for direct programming, flashing, and serial debugging. Includes auto-reset circuitry using a standard DTR/RTS transistor configuration.
  * **Port 2 (Native):** Direct native USB connection to the ESP32-S3 data pins.
* **Power Management:** Onboard 5V to 3.3V LDO regulation with jumper-selectable routing to easily isolate or select power sources during testing.
* **Signal Integrity & Protection:** Differential pairs for USB data lines are routed for 90Ω impedance. Both USB-C ports feature integrated ESD protection arrays to shield the ICs from voltage spikes.
* **User Interface:** Dedicated tactile switches for Boot and Reset, alongside independent Power and User-programmable status LEDs.
* **Aesthetics:** Custom exposed-copper ENIG (gold) logo implemented via precise solder mask cutouts on the top layer.

## Repository Structure
* **`Altium_Project/`**: Source files including the main project file (`.PrjPcb`), Schematics (`.SchDoc`), PCB Layout (`.PcbDoc`), and Custom Component Libraries (`.SchLib`, `.PcbLib`).
* **`Manufacturing_Outputs/`**: Production-ready `.zip` containing Gerber and NC Drill files, Pick and Place assembly data (`.csv`), and the full Bill of Materials (BOM).
* **`Datasheets/`**: Core technical reference documents, including the ESP32-S3 module datasheet.
* **`3D_Models/`**: STEP files used for the component bodies to ensure accurate 3D visualization and mechanical clearance checking.
* **`Schematic.pdf`**: A high-resolution PDF export of the circuit schematic for immediate browser viewing without requiring Altium Designer.

