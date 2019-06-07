# FMUv1 Pixhawk Open Hardware Design

> **General information about Pixhawk designs, schematics, reference hardware, FMU versions, licensing, and trademarks, and contributing to the project can be found in the repo [README](../README.md).**

This is the first Pixhawk FMU design, and was intended to be used with various piggyback boards, including an [IO](IOv1) board (the boards were combined into one package for the FMUv2 design).

> **Warning** This design is end-of-life.

## Design Files

The design is provided in [EAGLE](https://www.autodesk.com/products/eagle/overview) CAD files (can be viewed with the free version).

It consists of schematic files (*.sch) and includes open reference hardware PCB layouts (.brd). 
BOM management is performed using [Bob Starr's BOM-EX plugin](http://www.bobstarr.net/pages/downloads.html).

## Feature Overview

The PX4-FMU (Flight Management Unit).
- Cortex M4F micro-controller and flash memory for controlling flight and communications.
- SD memory card socket
- 3 axis gyro for determining attitude/orientation.
- 3 axis accelerometer.
- Compass (magnetometer).
- Barometric pressure sensor (altitude)
- Connection for external UBLOX LEA GPS
- Interconnections for adding stackable peripheral boards.
- USB, JTAG and Serial interfaces/connections.
- PPM-SUM RC radio inputs
- Servo outputs.
