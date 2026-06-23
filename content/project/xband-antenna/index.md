---
title: "Control of an X-band Antenna Mechanism"
summary: "Hands-on hardware project: control of a 2-axis X-band antenna pointing mechanism using Arduino, stepper motors, and a software-defined radio receive chain."
date: 2025-09-01
tags: ["Electronics", "Control", "Hardware", "Space"]
image:
  caption: ""
  focal_point: "Smart"
---

Hands-on hardware project to control the pointing of an X-band antenna mechanism, in the context of CubeSat ground-station operations.

**Topics covered:**
- Arduino-based control
- Electronics and signal chain (LNA, bias tee, downconversion stage, ADALM PlutoSDR)
- 2-axis control (X/Y modules) with NEMA 34 encoders and stepper rotators
- Stepper motor driving and closed-loop positioning

The system combines an RF receive chain (antenna â†’ LNA â†’ downconversion â†’ SDR) with a motion control chain (Teensy microcontroller â†’ stepper drivers â†’ NEMA 34 motors) to point the antenna accurately.

