# 🧠 HPA Triggerboard DevKit
<img width="584" height="622" alt="Trigger unit Completed" src="https://github.com/user-attachments/assets/3bfc1ab3-8754-4f1c-9170-ca44eac81204" />

Designed by Arthur – Tuka Customs™ and Eric - Sapo

This project showcases the end-to-end design of a fully programmable HPA triggerboard, developed from scratch as a complete electronics + product design solution for the airsoft community.
Every part of this device—from schematic architecture to PCB stack, component selection, mechanical clearances, firmware workflow, and user-oriented experience—was engineered with precision and professional methodology.

# 🎯 Project Overview

The Tuka Customs HPA Triggerboard DevKit is a logic-only electronic triggerboard built around the ATmega32U4 microcontroller.
Its main purpose is to give players, engineers, modders, and developers a platform to create, test, and experiment with new HPA features while preserving FCU safety and fairness.

This board does not drive solenoids.
It reads trigger and selector states, processes them through firmware, and allows expandable behaviors via customizable IO modules such as:

- LEDs

- Sensors

- OLED displays

- Battery monitors

- Research tools

- Custom reaction systems

- External modules & accessories

It’s the first airsoft triggerboard designed as an open development platform.

# 🛠 Design Goals
✔ Create a real development ecosystem for HPA

Instead of a simple “trigger switch board,” this project becomes a testing environment for firmware, accessories, and new gameplay ideas.

✔ Full programmability

Using the ATmega32U4’s native USB, users can upload custom code and connect the board directly to a PC.

✔ Expandable hardware

IO headers allow creators to attach their own modules, sensors, and UX elements.

✔ Clean mechanical integration

Designed around the tight geometry of V2 gearboxes with precise tolerances and a two-board sandwich system.

# 🌐 Hardware Architecture
- MCU: ATmega32U4

- Native USB support

- Digital + analog IO

- Arduino-compatible

- Perfect for expandable firmware design

- Power System

- USB-C input

- Onboard 5V regulator powering:

# The MCU

All expansion modules

Development accessories

Standalone use is fully supported—just plug USB-C.

Two-PCB Sandwich Design

The triggerboard consists of:

1. Main PCB

![top bottom](https://github.com/user-attachments/assets/3b222b2e-1d27-4261-8c2d-9e895a2eb644)

 - ATmega32U4

 - Trigger switch
  
 - IO expansion header

 - Selector switch
  
 - All decoupling + crystal network
 - 
![bottom bottom](https://github.com/user-attachments/assets/e54a9df5-fce2-4ae7-b094-ddf0aca3a467)

2. Top PCB

![bottom top](https://github.com/user-attachments/assets/bf08c7ed-d7a5-42f4-9ee6-f4aea2d835c2)

 - USB-C port

 - Power regulation

 - Firmware and serial communication system

 - Front headers connecting signals to main PCB

- Designed to clear gearbox trigger geometry

# 🔗 Signals and Connectivity
FCU JST-5 Standard Connectors

Compatible with Polarstar-style wiring:

Pin	Signal	Function
1	+5V	Powers regulator and system
2	Trigger	Read as digital input
3	Selector	Read as digital input
4	Poppet	Passthrough only
5	Nozzle	Passthrough only

Only trigger logic is interpreted.

Expandable IO Header

Exposes MCU pins for modules:

PB4, PB5, PB6, PB7 (Digital 8–11)

PF0, PF1 (Analog/Digital A4–A5)

VCC (regulated 5V)

GND

#  🧩 User Experience & Development Workflow

![top top](https://github.com/user-attachments/assets/c7b54218-f48a-4660-8020-bb50e83a1157)

1. Plug via USB-C

  - The board powers up
  
 - Exposes USB-serial
  
 - Accepts new firmware
  
 - Can run test modules (LEDs, OLEDs, sensors)

2. Test Trigger + Selector Logic

 - Observe reactions
  
 - Measure timing
  
 - Debug debounce
  
 - Prototype reaction systems

3. Add external modules

 - LED indicators
  
 - OLED UI
  
 - Shot counters
  
 - Vibration motors
  
 - R&D equipment

4. Drop inside replica & test in real movement
# 🔒 Future Production Model: Competition-Safe Version

- A second version will include:

  Locked firmware
  
  No USB reprogramming
  
  Signed firmware only
  
  Pre-approved functionality
  
  Ensuring the board is not used for unfair advantages in competitive matches.

# 📈 Product Contribution Summary

This project demonstrates:

<img width="696" height="519" alt="Screenshot 2025-05-27 033009" src="https://github.com/user-attachments/assets/6c64c88f-8e62-4cf6-b7ad-0c4324dd2348" />

✔ Electronics Engineering

  Full ATmega32U4 integration
  
  USB-C signal integrity
  
  Power regulation topology
  
  Decoupling + grounding strategy
  
  Dual-board communication design
  
<img width="689" height="768" alt="Screenshot 2025-05-27 033134" src="https://github.com/user-attachments/assets/99225e90-ade6-4847-b4d5-565bf865b9e7" />

✔ PCB Design

  2-layer optimization
  
  3D-validated mechanical placement
  
  High-precision sandwich headers
  
  Trigger clearance geometry
  
  Manufacturing-ready layout

✔ Industrial Design

  Form factor integrated into V2 gearbox
  
  Add-on compatibility
  
  Clean routing for reliability
  
  Expandability as a design principle

✔ Firmware & UX

  Modular IO logic
  
  Trigger analysis
  
  Reaction programming
  
  User-friendly testing workflow

🦾 Designed by Arthur – Tuka Customs™
