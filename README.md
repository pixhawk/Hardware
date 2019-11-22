# Pixhawk Hardware Designs

[![Join the chat at https://gitter.im/PX4/Hardware](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/PX4/Hardware?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) 

[Pixhawk](http://pixhawk.org) is an independent open-hardware project that aims to provide "the gold standard" for readily-available, hiqh-quality and low-cost autopilot hardware designs for the academic, hobby and developer communities.
Pixhawk supports multiple flight stacks: PX4 ® and ArduPilot ®.

> **Note** Designs are provided for a number of components used in unmanned vehicles, including: Autopilots (Flight Management Units - FMUs), ESCs (electronic speed controllers), optical flow sensors, etc.

## What are Open Hardware Designs?

The [Pixhawk project](https://pixhawk.org/) provides open hardware designs following the [OSHW 1.1 definition](https://www.oshwa.org/definition/).

In essence, this definition allows anyone to freely study, modify, distribute, make, and sell the designs (or hardware based on the designs) under the terms of a particular [open source licence](#licensing).

## Hardware Designs

Hardware designs delivered by the project are listed below.

<span id="fmu_designs"></span>
### FMU (Autopilot) Designs

Pixhawk FMU open designs include all information required to create an autopilot hardware product that is *firmware compatible* with other hardware created from the same design.
Manufacturers are encouraged to take the designs and create products that are best suited to a particular market or use case (e.g. for very small vehicles, or those that operate at environmental extremes).

> **Note** While a physical connector standard is not mandated, newer products generally follow the [Pixhawk Connector Standard](https://pixhawk.org/pixhawk-connector-standard/).


#### Design Specifications

Designs are *usually* specified in the form of *schematics* that show all included components (CPU, sensors, etc.), how they are connected, and their pin mappings.
They may also include a BOM (bill of materials).

> **Note** Not all designs deliver schematics.
  A minimal design needs to contain enough information for manufacturers to create a compatible products; this can also be achieved using a precise pinout definition and information about connections of internal/external busses, etc.

#### Open Reference Hardware

The project provides *open reference hardware/layouts* for **some** open designs, in some versions.
These are provided in the form of PCB layout files.

The reference hardware files are shared under the same [license](#licenses) as the associated open design, and hence may be used in the same way(s).

#### FMU Versions

The Pixhawk project has evolved the FMU design through a number of verisons.

These are named using the designation: FMUvX (e.g.: FMUv1, FMUv2, FMUv3, FMUv4, etc.).
Higher FMU numbers indicate that the board is more recent, but may not indicate increased capability (versions can be almost identical - differing only in connector wiring).

The versions are listed below (with a high level overview of the main differences).

Version | Year | Lead Product | CPU | Other
--- | --- | --- | --- | ---
[FMUv1](FMUv1/README.md) & [IOv1](IOv1) | 2012 | None | 168 MHz M4 | (Discontinued) Original Flight Management Unit and Separate I/O board.
[FMUv2](FMUv2/README.md) | 2013 | Pixhawk 1 | 168 MHz M4 | Single board with STM32427VI processor.
[FMUv3](FMUv3_REV_D/README.md) | 2015 | Pixhawk 2 | 168 MHz M4 | Redundant sensors. Identical to FMUv2, but usable flash doubled to 2MB.
[FMUv4](FMUv4/README.md) | 2015 | Pixracer | 168 MHz M4 | Increased RAM. Faster CPU. More serial ports. No IO processor.
FMUv4X | 2017 | Pixhawk 3 Pro | 168 MHz M4 | Slightly increased RAM. More serial ports. IO processor. Redundant sensors.
[FMUv5](FMUv5/README.md) | 2018 | Pixhawk 4 | 200 MHz M7 | New processor (F7). Much faster. More RAM. More CAN busses. Much more configurable.<br>> **Note** Minimum specification provided (pinout info, but no schematics).
FMUv5X | 2019 | Pixhawk 5X | 200 MHz M7 | Temp-calibrated, redundant sensors.


> **Note** Products based on Pixhawk designs are listed here: [PX4 User Guide > Pixhawk Series]( https://docs.px4.io/master/en/flight_controller/pixhawk_series.html#pixhawk-series).


#### Derived FMU Products

Commercial products that are *derived* (under the terms of the open source license) from the Pixhawk FMU designs must provide their schematics and other information.

Relevant products are listed below:

- [MindPX V2 Hardware](MindPXv2/README.md)


### Sapog ESC

- [Sapog ESC](https://github.com/PX4/sapog) Hardware - The directory [sapog_reference_hardware](sapog_reference_hardware/README.md) contains the reference hardware design for the Sapog ESC firmware.

### Other

- [AIRSPEEDv1](AIRSPEEDv1) - 
- [FLOWv1](FLOWv1)
- [IMUv3_REV_C](IMUv3_REV_C)
- [PSMv3_REV_C](PSMv3_REV_C)

<span id="dev_call"></span>
## Dev Call

Pixhawk standards are developed in a weekly public developer call.

The call is shown in the [Dronecode calendar](https://www.dronecode.org/calendar/) as: *Pixhawk Hardware Standards Weekly Call* (all call details are in the entry).


<span id="licensing"></span>
## Licensing and Trademarks

Pixhawk project schematics and reference designs are licensed under [CC BY-SA 3](https://creativecommons.org/licenses/by-sa/3.0/legalcode).

The license allows you to use, sell, share, modify and build on the files in almost any way you like - provided that you give credit/attribution, and that you share any changes that you make under the same open source license (see the [human readable version of the license](https://creativecommons.org/licenses/by-sa/3.0/) for a concise summary of the rights and obligations).

> **Note** Boards that are *derived directly* from Pixhawk schematic files (or reference boards) must be open sourced.
  They can't be commercially licensed as proprietary products.

Manufacturers can create (compatible) *fully independent products* by first generating fresh schematic files that have the same pin mapping/components as the FMU designs.
Products that are based on independently created schematics are considered original works, and can be licensed as required.

<span id="trademarks"></span>
## Trademarks

The term *Pixhawk* is a trademark, and may not be used in product names without explicit permission from the trademark owner.

Typically this trademark is granted to the first board based on a particular FMU design and/or boards that use Pixhawk open reference hardware layouts.

> **Note** A "Pixhawk" is an autopilot that has been been given permission to use the Pixhawk trademark in its name.
  While other boards are based on the "Pixhawk FMU Standard", the are not *strictly speaking* "Pixhawks".

