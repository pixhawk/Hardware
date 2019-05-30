# Pixhawk Hardware Designs

[![Join the chat at https://gitter.im/PX4/Hardware](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/PX4/Hardware?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) 

[Pixhawk](http://pixhawk.org) is an independent open-hardware project that aims to provide "the gold standard" for readily-available, hiqh-quality and low-cost autopilot hardware designs for the academic, hobby and developer communities.
Pixhawk supports multiple flight stacks: PX4 ® and ArduPilot ®.

> **Note** Designs are provided for a number of components used in unmanned vehicles, including: Autopilots (Flight Management Units - FMUs), ESCs (electronic speed controllers), optical flow sensors, etc.

## What are Open Hardware Designs?

The [Pixhawk project](https://pixhawk.org/) provides open hardware designs following the [OSHW 1.1 definition](https://www.oshwa.org/definition/).

In essence, this definition allows anyone to freely study, modify, distribute, make, and sell the designs (or hardware based on the designs) under the terms of a particular open source licence (you can find more about the [open source licence](#licensing) we use below).

## Hardware Designs

Hardware designs delivered by the project are listed below.

<span id="fmu_designs"></span>
### FMU (Autopilot) Designs

Pixhawk FMU open designs include all information required to create an autopilot hardware product that is *firmware compatible* with other hardware created from the same design.
Manufacturers are encouraged to take the designs and create products that are best suited to a particular market or use case (e.g. for very small vehicles, or those that operate at environmental extremes).

> **Note** While a physical connector standard is not mandated, newer products generally follow the [Pixhawk Connector Standard](https://pixhawk.org/pixhawk-connector-standard/).


#### Design Format

Designs are *usually* specified in the form of *schematics* that show all included components (CPU, sensors, etc.), how they are connected, and their pin mappings.
They may also include a BOM (bill of materials).

> **Note** Not all designs deliver schematics.

#### Reference Hardware

The project provides *reference hardware/layouts* for **some** based on some open designs, in the form of PCB layout files.

These are shared under the same [license](#licenses) as the open design, and hence may be used in the same ways.

#### FMU Versions

The Pixhawk project has evolved the FMU design through a number of verisons.

These are named using the designation: FMUvX (e.g.: FMUv1, FMUv2, FMUv3, FMUv4, etc.).
Higher FMU numbers indicate that the board is more recent, but may not indicate increased capability (versions can be almost identical - differing only in connector wiring).

The designs listed below (with a high level overview of the main differences).

Version | Description
--- | ---
[FMUv1](FMUv1/README.md) & [IOv1](IOv1) | (Discontinued) Original Flight Management Unit and Separate I/O board.
[FMUv2](FMUv2/README.md) | Single board with STM32427VI processor.
[FMUv3](FMUv3_REV_D/README.md)| Identical to FMUv2, but usable flash doubled to 2MB.
[FMUv4](FMUv4/README.md) | Increased RAM. Faster CPU. More serial ports. No IO processor
FMUv4-PRO | Slightly increased RAM. More serial ports. IO processor.
[FMUv5](FMUv5/README.md) | New processor (F7). Much faster. More RAM. More CAN busses. Much more configurable.<br>> **Note** Minimum specification provided (pinout info, but no schematics).



### Sapog ESC

- [Sapog ESC](https://github.com/PX4/sapog) Hardware - The directory [sapog_reference_hardware](sapog_reference_hardware/README.md) contains the reference hardware design for the Sapog ESC firmware.

### Other

- [AIRSPEEDv1](AIRSPEEDv1) - 
- [FLOWv1](FLOWv1)
- [IMUv3_REV_C](IMUv3_REV_C)
- [PSMv3_REV_C](PSMv3_REV_C)


## Derived Autopilot Products

The following boards are commercial products that are *derived* from the Pixhawk FMU designs above (information is provided here under the terms of the open source license):

- [MindPX V2 Hardware](MindPXv2/README.md)

> **Note** Many other products are based on the FMU designs, but are not "derived products" under the terms of the license (and are hence not listed here). For other hardware see [PX4 User Guide > Pixhawk Series]( https://docs.px4.io/master/en/flight_controller/pixhawk_series.html#pixhawk-series).



<span id="licensing"></span>
### Licensing and Trademarks

Pixhawk project schematics and reference designs are licensed under [CC BY-SA 3](https://creativecommons.org/licenses/by-sa/3.0/legalcode).

The license allows you to use, sell, share, modify and build on the files in almost any way you like - provided that you give credit/attribution, and that you share any changes that you make under the same open source license (see the [human readable version of the license](https://creativecommons.org/licenses/by-sa/3.0/) for a concise summary of the rights and obligations).

> **Note** Boards that are *derived directly* from Pixhawk schematic files (or reference boards) must be open sourced. 
  They can't be commercially licensed as proprietary products.

Manufacturers can create (compatible) *fully independent products* by first generating fresh schematic files that have the same pin mapping/components as the FMU designs.
Products that are based on independently created schematics are considered original works, and can be licensed as required.

Product names/brands can also be trademarked. Trademarked names may not be used without the permission of the owner.

> **Tip** *Pixhawk* is a trademark, and cannot be used in product names without permission.
