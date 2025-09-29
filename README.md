# Lab 1: GPIO control on STM32F103C6

This repository contains my solutions for **Lab 1 – LED Animations & GPIO Programming** in the Microcontroller & Microprocessor course. 
All projects are developed using **STM32CubeIDE** and simulated with **Proteus**.

---

## Overview

The lab introduces **GPIO programming** on the STM32F103C6 microcontroller and progressively builds from simple LED toggling to more complex systems such as **traffic lights**, **countdown timers**, and an **analog clock with 12 LEDs**.

Key concepts:

- Configuring STM32 pins as **GPIO Output** using STM32CubeMX.
- Controlling **active-low LEDs** (negative pin to MCU pin).
- Driving **7-segment common anode displays** (logic `0` lights a segment).
- Using **HAL** functions (`HAL_GPIO_WritePin`, `HAL_GPIO_TogglePin`) for pin control.
- Structuring code with helper functions and enums for state machines.

---

## Lab Exercises Implemented

| Exercise | Description |
|----------|-------------|
| **Ex 1** | Blink two LEDs (PA5, PA6) alternately every 2s. |
| **Ex 2** | Simulate a **3-LED traffic light** (RED 5 s → GREEN 3 s → YELLOW 2 s). |
| **Ex 3** | Extend to a **4-way traffic light** with 6 LEDs per direction (vertical & horizontal). |
| **Ex 4** | Add a **single 7-segment display** driven by PB0–PB6; implement `display7SEG(int num)`. |
| **Ex 5** | Integrate the 7-segment display to show **countdown timers** for each traffic light direction. |
| **Ex 6-10** | Build an **analog clock** with 12 LEDs (PA4–PA15): – **`clearAllClock()`** turns all LEDs off – **`setNumberOnClock(num)`** lights one LED – Final clock shows **hour, minute, second** simultaneously. |

---
