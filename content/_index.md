+++
title = 'Home'
+++

# Unbound Silicon

## Software for silicon, not platforms.

Platform-independent embedded drivers and hardware interfaces written in C.

---

## Write for the hardware, not the platform.

Embedded devices do not fundamentally change because the microcontroller connected to them changes.

An RFM12B is still an RFM12B whether it is connected to an AVR, STM32, ESP32, or another system entirely. The register map, commands, timing requirements, and behavior of the device remain the same.

Unbound Silicon drivers are designed around that idea.

Platform-specific operations such as SPI, I²C, GPIO, timing, and interrupts remain outside the driver whenever practical. The application provides those services through a well-defined Hardware Abstraction Layer (HAL), while the driver remains focused on the hardware it was written to control.

The result is code intended to be portable, understandable, and useful beyond a single development board or software framework.

---
