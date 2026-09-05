# STM32F401RE Evaluation Board

Two-layer STM32F401RE (LQFP64) evaluation board designed in KiCad, built as
a solo entry for the **Mixed Traces PCB Design Competition**, hosted by
Mixed Signals (Electronics Association of MEC).

# Overview

A compact, self-contained STM32F401RE dev board inspired by the
NUCLEO-F401RE reference design, built to fit within a 100mm x 100mm,
two-layer PCB. Per the competition rules, an on-board ST-LINK debugger is
not required — programming and debugging are handled through an external
SWD header instead.

## Features

- STM32F401RET6 (LQFP64) microcontroller
- USB-C power input with CC1/CC2 pull-downs and USBLC6-2SC6 ESD protection
- NCP1117-3.3 LDO regulation
- 8MHz HSE crystal (derives both the 84MHz system clock and 48MHz USB clock)
- External SWD header for programming/debugging
- UART, SPI, and I2C headers
- 34 GPIO broken out across four expansion headers, each with 3V3/GND
  reference pins
- Dedicated power breakout header (VBUS, 3V3, GND)
- User + reset buttons, user + power LEDs
- Full ground plane pour on both copper layers

# Repository structure

```
hardware/     KiCad project, schematic, and PCB layout files
docs/         Schematic PDF export, PCB renders, BOM, design description
progress/     Competition progress-checkpoint submission
```

# Tools

Designed entirely in [KiCad](https://www.kicad.org/) 9.

# Status

Entered in the Mixed Traces PCB Design Competition — progress checkpoint
submitted 5 September 2026, final submission due 15 September 2026.

# License

Hardware design files in this repository are licensed under the
[CERN Open Hardware Licence Version 2 - Permissive (CERN-OHL-P-2.0)](LICENSE).

# Author

Adarsh S — [Payload Circuits](https://github.com/PayloadCircuits)
