+++
title = 'RFM12 / RFM12B'
driver_id = 'rfm12'
show_examples = false
+++

A portable C driver for the HopeRF RFM12 and RFM12B ISM-band transceivers.

The goal of my RFM12 driver is to provide a modern, hardware-independent, and well-documented C library that abstracts the device's low-level command interface into a clean, intuitive API.

## Overview

The RFM12 and RFM12B are highly configurable ISM-band transceivers controlled through a 16-bit SPI command interface. While the devices provide considerable flexibility, using them directly requires an application to manage command encoding, configuration fields, operating modes, and device status.

The RFM12 driver moves those device-specific details into the library and exposes them through a higher-level C API. Platform-specific operations, such as SPI communication, remain outside the driver so the same library can be used with different microcontrollers and hardware environments.

## Features

- Hardware-independent C implementation with an abstraction layer for platform-specific SPI communication.
- Manages RFM12 command and register bit fields through simple, concise API functions.
- Support for multiple independent RFM12/RFM12B instances.
- Explicit receive, transmit, idle, standby, and sleep operating modes.
- Radio status and diagnostic information exposed through simple API functions.
- No dynamic memory allocation is required on the target MCU.

## Tested Platforms

The hardware abstraction layer allows the RFM12 driver to be used across different microcontroller and hardware platforms. Development and testing have currently been performed on:

- AVR
- STM32

## Resources

- **Source Code** — [UnboundSilicon/rfm12](https://github.com/UnboundSilicon/rfm12)
- **Documentation** — [link to be added]
- **Example Driver Code** — [RFM12 Driver Ping-Pong Example](https://github.com/UnboundSilicon/rfm12/tree/main/examples/ping-pong)
- **Datasheet** — [RFM12B.pdf](https://github.com/UnboundSilicon/rfm12/blob/main/datasheets/RFM12B.pdf)
- **Manufacturer Example Code** — [RFM12B_code.pdf](https://github.com/UnboundSilicon/rfm12/blob/main/datasheets/RFM12B_code.pdf)
