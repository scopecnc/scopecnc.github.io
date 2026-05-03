---
layout: page
title: About
subtitle: The ScopeCNC Project
---

## What is ScopeCNC?

ScopeCNC is a custom-built CNC microscope platform designed for automated mineral specimen photography. It enables precise grid-based navigation, automated focus stacking, and high-resolution imaging of geological specimens.

## Project Goals

- **Automated Imaging** — Photograph entire specimen trays with consistent focus and lighting
- **Focus Stacking** — Capture multiple focal planes and composite them into sharp images
- **Specimen Cataloging** — Navigate named grid positions with stored coordinates
- **Open Source** — All hardware designs, firmware, and software freely available

## Architecture

The system uses a two-processor architecture:

1. **Raspberry Pi 4** — Runs the PyQt5 GUI, handles video capture, manages specimen databases, and sends motion commands
2. **Teensy 4.1** — Receives serial commands and drives servos/steppers with microsecond-precision PWM timing

Communication flows over USB serial using a custom binary protocol with CRC16 error checking.

## Who Built This?

ScopeCNC was developed as a personal project for automated mineralogy photography. The platform is designed to be reproducible by anyone with basic electronics and 3D printing capabilities.
