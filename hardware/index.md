---
layout: page
title: Hardware
subtitle: Mechanical and Electrical Design
---

## System Components

### Motion Control

- **X/Y Stage** — Linear actuators for specimen tray positioning
- **Z Axis** — Fine-focus stepper motor for focal plane control
- **Teensy 4.1** — Microcontroller generating PWM signals for servos and step/direction for steppers

### Electronics

- **Power Distribution** — 12V main supply with regulated 5V and 3.3V rails
- **LED Lighting** — PWM-controlled ring light with adjustable brightness
- **HDMI Capture** — USB capture card feeding microscope video to the Pi

### Schematics

Detailed wiring diagrams and signal routing are available in the [documentation repository](https://github.com/scopecnc/rpi4-firmware/tree/main/schematics).

---

## Pin Assignments

See the [Teensy pinout reference](https://github.com/scopecnc/teensy-firmware/blob/main/teensy_pinout.md) for complete pin mapping.
