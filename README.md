# Custom Dual-Rail Boost Regulator & Embedded Sensor PCB

**Focus:** Power Delivery | Thermal Validation | SMD Manufacturing

While this system functions as an ultrasonic range finder, the core engineering focus of this repository is the design, fabrication, and thermal validation of a custom 2-layer 3.3V and 5.0V boost regulator PCB. The board was architected in Fusion 360 to reliably supply an MSP430 microcontroller and I2C peripherals under strict thermal and voltage constraints.

## ⚡ Power Design & Hardware Validation
*   **Power Architecture:** Designed a 2-layer boost regulator PCB optimized for a 150 mA continuous load, supplying both 3.3V and 5.0V rails for mixed-signal components.
*   **Thermal Validation:** Conducted infrared thermography testing on the physical board under load, verifying excellent heat dissipation with a measured peak regulator temperature of just 28.9°C.
*   **Signal Integrity:** Validated power delivery quality using an oscilloscope, measuring and verifying a voltage ripple of less than 25mV to ensure stable operation of the MSP430G2553.

## 🏭 Manufacturing & Firmware Integration
*   **SMD Assembly:** Generated full Pick-and-Place (PnP) files and executed complete surface-mount device (SMD) assembly and thermal reflow using a Neoden YY1 machine.
*   **Embedded Control:** Developed embedded C firmware in Code Composer Studio (CCS) to handle ultrasonic distance calculations and drive a 16x2 I2C LCD display.

## 🗂️ Repository Structure
*(Note: Upload your files into these folders)*
*   **`/Hardware`**: Fusion 360 electronic design files, schematics, and board layouts.
*   **`/Fabrication`**: Gerber files, BOM, and Neoden YY1 Pick-and-Place (PnP) generation files.
*   **`/Firmware`**: MSP430G2553 embedded C code and CCS project files.
