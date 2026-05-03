---
layout: home
title: ScopeCNC
subtitle: Open-Source CNC Microscope Platform
---

# Welcome to ScopeCNC

ScopeCNC is an open-source CNC-controlled microscope platform built for automated specimen imaging, focus stacking, and grid-based sample navigation. The system combines a Raspberry Pi 4 with a Teensy 4.1 microcontroller to deliver precise 3-axis motion control with sub-micron positioning.

---

## Quick Links

<div class="row">
<div class="col-md-4">
<div class="card text-center p-3 mb-3" style="border: 2px solid #0f3460; border-radius: 10px;">
<h3>🔧 Hardware</h3>
<p>Servo/stepper control, power distribution, and wiring schematics</p>
<a href="hardware/" class="btn btn-primary">View Hardware</a>
</div>
</div>
<div class="col-md-4">
<div class="card text-center p-3 mb-3" style="border: 2px solid #0f3460; border-radius: 10px;">
<h3>💻 Software</h3>
<p>PyQt5 GUI, Teensy firmware, and communication protocol</p>
<a href="software/" class="btn btn-primary">View Software</a>
</div>
</div>
<div class="col-md-4">
<div class="card text-center p-3 mb-3" style="border: 2px solid #0f3460; border-radius: 10px;">
<h3>📸 Gallery</h3>
<p>Photos of the build, specimens, and focus-stacked images</p>
<a href="gallery/" class="btn btn-primary">View Gallery</a>
</div>
</div>
</div>

---

## System Overview

| Component | Description |
|-----------|-------------|
| **Controller** | Raspberry Pi 4 (4GB) running PyQt5 GUI |
| **Motion** | Teensy 4.1 driving servos and stepper motors |
| **Axes** | X, Y (specimen stage), Z (focus) |
| **Communication** | USB serial protocol at 115200 baud |
| **Display** | HDMI capture of microscope video feed |
| **Lighting** | PWM-controlled LED ring with brightness control |

---

## Source Code

- [RPI4 Firmware](https://github.com/scopecnc/rpi4-firmware) — Python control software
- [Teensy Firmware](https://github.com/scopecnc/teensy-firmware) — C++ microcontroller code

---

*ScopeCNC is released under the [MIT License](https://github.com/scopecnc/rpi4-firmware/blob/main/LICENSE).*
