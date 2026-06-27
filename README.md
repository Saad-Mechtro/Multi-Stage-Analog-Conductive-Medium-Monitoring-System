# Multi-Stage Analog Conductive Medium Status Monitoring System

A hardware-based analog liquid level monitoring system designed using the **LM324 Quad Operational Amplifier**. The project detects four different conductive liquid levels, provides progressive LED indication, and activates a buzzer at the critical level. The complete system was designed, simulated, fabricated on a custom PCB, and successfully tested.

---

## Project Overview

This project was developed as part of the **Electric Circuit Analysis (ECA)** course in the **BS Mechatronics Engineering** program.

Unlike microcontroller-based liquid level monitoring systems, this design uses only analog electronic components. The system detects conductive liquid levels using sensing probes and compares them against reference voltages generated through a resistor ladder network.

As the liquid level rises, LEDs illuminate one by one. When the highest level is reached, a buzzer is activated to indicate a critical condition.

---

## Features

* Four-stage conductive liquid level detection
* Pure analog circuit (No Arduino or Microcontroller)
* LM324 Op-Amp based voltage comparator
* Progressive LED indication
* Critical level buzzer alert
* Single-layer custom PCB design
* Proteus ISIS simulation
* Proteus ARES PCB layout
* Hardware implementation and testing

---

## Components Used

| Component              | Quantity |
| ---------------------- | -------- |
| LM324 Quad Op-Amp      | 1        |
| LEDs                   | 4        |
| 47kΩ Resistors         | 8        |
| 220Ω Resistors         | 4        |
| 10kΩ Resistors         | 5        |
| Electrolytic Capacitor | 1        |
| Ceramic Capacitor      | 1        |
| Diode                  | 1        |
| Passive Buzzer         | 1        |
| PCB                    | 1        |
| Sensor Connector       | 1        |
| 12V DC Supply          | 1        |

---

## Working Principle

The monitoring system consists of four conductive sensing probes placed at different heights.

When the conductive liquid reaches a probe, the corresponding input voltage increases.

The LM324 compares this voltage with predefined reference voltages generated using a resistor ladder.

Operation:

* Stage 1 → LED 1 ON
* Stage 2 → LED 2 ON
* Stage 3 → LED 3 ON
* Stage 4 → LED 4 ON + Buzzer ON

This provides a simple and reliable indication of liquid level without using any programmable controller.

---

# Circuit Diagram

---

# PCB Layout

---

# 3D PCB Design

---

# Hardware Prototype

### Front View

### Back View

---

## Challenges Faced

During development, several practical issues were encountered:

* Floating sensor inputs caused false triggering.
* One capacitor was faulty and had to be replaced.
* Incorrect IC orientation during initial testing.
* PCB debugging after fabrication.
* Added pull-down resistors for stable sensor inputs.
* Added a decoupling capacitor to reduce electrical noise.

After troubleshooting, the circuit operated successfully.

---

## Software Used

* Proteus ISIS
* Proteus ARES

---

## Applications

* Water Tank Level Monitoring
* Chemical Storage Tanks
* Industrial Liquid Monitoring
* Educational Analog Electronics Projects
* Laboratory Demonstrations

---

## Future Improvements

* LCD Display
* IoT Monitoring
* GSM Notifications
* Automatic Pump Control
* Wireless Monitoring
* Mobile Application Integration

---

## Repository Structure

```text
├── Images
├── Proteus Files
├── Documentation
├── README.md
├── LICENSE
└── .gitignore
```

---

## Author

**Hafiz Muhammad Saad Habib**

BE Mechatronics Engineering

Air University, Islamabad

---

## License

This project is released under the MIT License.
