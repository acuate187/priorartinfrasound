# Low-Cost Infrasound-Based Collision Avoidance System

Status: Public domain disclosure under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/)

Disclosure Date: April 18, 2025  
Inventor: Colton Ryan McMaster  
Location: Texas, USA

---

## Summary

This system uses low-frequency infrasound (20–50Hz), MEMS microphone arrays, and real-time spectrogram analysis to detect and prevent collisions in industrial vehicles. It achieves performance comparable to high-cost LiDAR/RADAR systems with < $20 in parts.

> Key Innovation:  
> Using sub-50Hz omnidirectional acoustic waves and Doppler-based predictive math for momentum vectoring — no vision, no moving parts, no heavy compute.

---

## Why This Matters

- LiDAR & vision-based systems are expensive and fail in dust, fog, vibration.
- Infrasound propagates omnidirectionally, penetrates through obstacles, and doesn’t require human-detectable signals.
- True real-time math-based detection using basic physics and FFT analysis — no AI, no black boxes, no data fuzzing.

---

## System Overview

- Emitter: 30Hz Piezo transducer
- Receiver: 4x MEMS microphones (90° array)
- Processor: Raspberry Pi Pico running custom FFT
- Output: Collision warning, brake trigger, CAN bus integration

---

## Operational Flow

1. Emit 30Hz pulse
2. Record echoes via microphone array
3. Perform FFT to detect shifts
4. Calculate velocity & Time-to-Collision (TTC)
5. Trigger response if TTC < 2.0s

---

## Legal Notes

This repository serves as a public, timestamped disclosure under 35 USC §102(b)(1) as prior art.  
All technical details are enabled and can be incorporated by reference into any future filings.

---

## Contact

Want to collaborate, improve, or commercialize?  
Email: ryancolton063@gmail.com
