
# **LogicDriven-Motion-RGB**


[![GitHub](https://img.shields.io/badge/GitHub-ODARI--CHARLES1-181717?style=for-the-badge&logo=github)](https://github.com/ODARI-CHARLES1)
[![Portfolio](https://img.shields.io/badge/Portfolio-View-blue?style=for-the-badge&logo=google-chrome)](https://charles.k.odari.portfolio.thegtm.or.ke/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin)](https://ke.linkedin.com/in/odari-kibisi-charles-329b19331)
[![Email](https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:daymondodari68@gmail.com)

---
![Uploading image.png…]()


## **Project Overview**

**Combinational-Motor-RGB** is a **hardware project** that combines **pure combinational logic circuits** to control:

* Multi-directional **motor movement** (Up, Down, Left, Right)
* **RGB LED lighting patterns** with multiple colors
* **Timing control** using **three independent square wave signals**

This project is  **microcontroller-free** , relying entirely on:

* Logic gates (AND, OR, NOT)
* Decoders / Encoders
* Multiplexers / Demultiplexers
* Comparators and adders
* Square-wave signal generators

It demonstrates **real-world combinational circuit design** for automation and robotics applications.

---

## **Features**

| Feature                 | Description                                                     |
| ----------------------- | --------------------------------------------------------------- |
| Motor Control           | X-Y movement using H-bridges driven by combinational logic      |
| RGB Control             | 8-color LED patterns selectable via combinational decoders      |
| Multi-Frequency Signals | Three independent square-wave signals for timing and modulation |
| Safety Logic            | Prevents conflicting motor commands using logic gates           |
| Expandable              | Can be scaled to more motors or more complex LED patterns       |

---

## **Circuit Diagram**

```text
[Direction Switches] ──> [2-to-4 Decoder] ──> [Motor H-Bridge Control]
[Color Switches]     ──> [3-to-8 Decoder] ──> [RGB LEDs]
[Logic Gates] ──> Combine signals to prevent conflicts & sync LEDs with motors
[Square Wave Module] ──> Drives motor PWM & LED blinking
```

> Full Proteus schematic and simulation files are included in `/schematics`.

---

## **Technologies / Components Used**

[![Verilog](https://img.shields.io/badge/Verilog-FD5F00?style=for-the-badge&logo=verilog&logoColor=white)](https://chatgpt.com/c/69d3f66f-e010-8325-b4b6-64230833bb4c)
[![Logic Gates](https://img.shields.io/badge/LogicGates-007ACC?style=for-the-badge&logo=logicdesign&logoColor=white)](https://chatgpt.com/c/69d3f66f-e010-8325-b4b6-64230833bb4c)
[![H-Bridge](https://img.shields.io/badge/H--Bridge-FF6F00?style=for-the-badge)](https://chatgpt.com/c/69d3f66f-e010-8325-b4b6-64230833bb4c)
[![EEPROM](https://img.shields.io/badge/EEPROM-9C27B0?style=for-the-badge)](https://chatgpt.com/c/69d3f66f-e010-8325-b4b6-64230833bb4c)
[![Oscillator](https://img.shields.io/badge/Oscillator-4CAF50?style=for-the-badge)](https://chatgpt.com/c/69d3f66f-e010-8325-b4b6-64230833bb4c)

---

## **Modules**

### **1. Motor Control Module**

* Uses **2-to-4 decoder** to select motor direction.
* H-Bridge ensures safe rotation  **up/down or left/right** .
* AND/OR logic prevents  **conflicting signals** .

### **2. RGB LED Module**

* **3-to-8 decoder** selects RGB LED colors.
* Combined with square-wave module for  **blinking patterns** .

### **3. Square Wave Generator Module**

* Provides **3 independent frequencies** from a single chip.
* Feeds motor control PWM and LED blink circuits.

---

## **Usage**

1. Clone the repository:

```bash
git clone https://github.com/ODARI-CHARLES1/LogicDriven-Motion-RGB
```

2. Open the **Proteus project** in `/schematics`.
3. Adjust **switches** to select motor direction and LED colors.
4. Observe motor movement and RGB patterns.
5. Optional: Modify **square-wave module** to change frequency outputs.

---

## **Future Enhancements**

* Add **speed control** using variable frequency inputs.
* Expand to **more RGB LEDs** or multi-color patterns.
* Integrate **additional motors** for robotic arm applications.
* Add **emergency stop logic** for industrial use.

---

## **License**

This project is licensed under the **MIT License** – see the [LICENSE](https://chatgpt.com/c/LICENSE) file for details.
