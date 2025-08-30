# 24V to 5V Buck Converter

This repository contains the design files for a **24V to 5V buck converter** based on the LMR14010ADDCT IC.

---

## Key Features

* **Input Voltage:** 24V DC
* **Output Voltage:** 5V DC
* **High Efficiency:** Utilizes a modern switching regulator IC (**LMR14010ADDCT**) for high power efficiency.
* **Compact Design:** The PCB layout is designed to be small with mounting to easily integrate into other projects.
* **Robust Output:** Multiple output capacitors and a well-designed feedback loop to ensure a stable and low-ripple 5V supply.

---

## Project Files

* `24V_to_5V_Buck_Converter.PrjPcb`: Altium Project file
* `24V_to_5V_Buck_Converter.SchDoc`: Schematic of the buck converter
* `24V_to_5V_Buck_Converter.PcbDoc`: PCB layout design

---

## Component Breakdown

The circuit is centered around the **LMR14010ADDCT buck regulator IC (U1)**. Key components include:

* **U1 (LMR14010ADDCT):** The buck regulator IC that efficiently steps down the input voltage to a stable 5V output.
* **L1 (22µH Inductor):** Stores energy during the on-cycle and releases it during the off-cycle to smooth the current.
* **D1 (B240-13-F):** A Schottky diode that provides a path for the inductor current when the IC's switch is off.
* **C1 (0.47nF):** A bootstrap capacitor that powers the IC's internal high-side switch driver.
* **C2 (4.7µF):** The input capacitor that stabilizes the input voltage for the IC.
* **C3, C4, C5 (22µF, 0.1µF, 0.01µF):** Output capacitors that filter the output voltage to provide a clean and stable 5V supply.
* **R1 (86.6KΩ), R2 (55KΩ), R3 (10KΩ), and R4 (10KΩ):** Resistors for voltage divider to set the final 5V output.
* **P1 and P2:** Standard JST 2-pin connectors for the 24V input and 5V output.