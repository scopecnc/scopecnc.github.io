---
layout: page
title: Software
subtitle: Control Software and Firmware
---

## RPI4 Control Software

The main application is a PyQt5-based GUI (`scope_gui.py`) running on Raspberry Pi 4. It provides:

- **Live Video Feed** — HDMI capture displayed in real-time
- **Motion Control Panel** — Jog buttons, coordinate display, home/park functions
- **Specimen Grid** — Named positions with stored X/Y/Z coordinates
- **Focus Stacking** — Automated Z-axis sweep with image capture
- **LED Control** — Brightness slider with min/max limits
- **Tray Management** — Load/save specimen tray configurations as JSON

### Source Code

[View RPI4 source on GitHub →](https://github.com/scopecnc/rpi4-firmware)

---

## Teensy Firmware

The Teensy 4.1 firmware handles real-time motion control:

- **Serial Protocol** — Binary message format with CRC16 checksums
- **PWM Generation** — Microsecond-precision servo positioning
- **Stepper Control** — Acceleration/deceleration profiles for smooth motion
- **Safety Limits** — Software endstops and watchdog timer
- **Diagnostics** — Built-in test modes for hardware verification

### Source Code

[View Teensy source on GitHub →](https://github.com/scopecnc/teensy-firmware)

---

## Communication Protocol

The Pi and Teensy communicate over USB serial at 115200 baud using a custom binary protocol. See the [protocol specification](https://github.com/scopecnc/teensy-firmware/blob/main/PROTOCOL.md) for message formats and command reference.
