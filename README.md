# Pixhawk Hardware Designs

[![Join the chat at https://gitter.im/PX4/Hardware](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/PX4/Hardware?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) 

[Pixhawk](http://pixhawk.org) is an independent open-hardware project that aims to provide the standard for readily-available, hiqh-quality and low-cost autopilot hardware designs for the academic, hobby and developer communities. Pixhawk supports multiple flight stacks: PX4 ® and ArduPilot ®.

## What is an Open Design?

The [Pixhawk project](https://pixhawk.org/) provides open designs following the OSHW 1.1 definition.

Designs are (typically) specified in the form of *schematics* that show all included components (CPU, sensors, etc.), how they are connected, and their pin mappings. 
They may also include a BOM (bill of materials).

> **Tip** A minimum design must include all information required for a manufacturer to create a hardware product that is *firmware compatible* with other hardware created to the same design.
  This might not be a full schematic, but must include a clear pinout definition of all components, information about I2C buses (e.g. which are internally available vs what is attached internally), etc.

The project also delivers *reference hardware* for some open designs.
If created, these are delivered as PCB layout files, and shared under the same [license](#licenses).

Manufacturers are encouraged to take the open designs (and/or open reference hardware) and create firmware-compatible products that are best suited to a particular market or use case (the physical layout/form factor not part of the open specification).

> **Note** While a physical connector standard is not mandated, newer products generally follow the [Dronecode<sup>&reg;</sup> Autopilot Connector Standard](https://wiki.dronecode.org/workgroup/connectors/start).


## Hardware Designs

### FMU (Autopilot) Designs

The project has created a number of different open designs for flight management units (autopilot hardware). 
These are named using the designation: FMUvX (e.g.: FMUv1, FMUv2, FMUv3, FMUv4, etc.).
Higher FMU numbers indicate that the board is more recent, but may not indicate increased capability (versions can be almost identical - differing only in connector wiring).

The designs listed below (with a high level overview of main differences): 

- [FMUv1](FMUv1/README.md) & [IOv1](IOv1) - (Discontinued) Original Flight Management Unit and Separate I/O board.
- [FMUv2](FMUv2/README.md) - Single board with STM32427VI processor.
- [FMUv3](FMUv3_REV_D/README.md) - Identical to FMUv2, but usable flash doubled to 2MB.
- [FMUv4](FMUv4/README.md) - Increased RAM. Faster CPU. More serial ports. No IO processor
- FMUv4-PRO - Slightly increased RAM. More serial ports. IO processor <!-- is this design compatible - is it a reference? -->
- [FMUv5](FMUv5/README.md) - New processor (F7). Much faster. More RAM. More CAN busses. Much more configurable.
  > **Note** Minimum specification provided (pinout info, but no schematics).


### Sapog ESC

- [Sapog ESC](https://github.com/PX4/sapog) Hardware - The directory [sapog_reference_hardware](sapog_reference_hardware/README.md) contains the reference hardware design for the Sapog ESC firmware.

### Other

- [AIRSPEEDv1](AIRSPEEDv1) - 
- [FLOWv1](FLOWv1)
- [IMUv3_REV_C](IMUv3_REV_C)
- [PSMv3_REV_C](PSMv3_REV_C)


## Autopilot Products

The following boards are commercial products that are *derived* from the Pixhawk FMU designs above (information is provided here under the terms of the open source license):

- [MindPX V2 Hardware](MindPXv2/README.md)

> **Note** Many other products are based on the FMU designs, but are not "derived products" under the terms of the license (and are hence not listed here). For other hardware see [PX4 User Guide > Pixhawk Series]( https://docs.px4.io/master/en/flight_controller/pixhawk_series.html#pixhawk-series).



### Licensing and trademarks

Pixhawk project schematics and reference designs are licensed under [CC BY-SA 3](https://creativecommons.org/licenses/by-sa/3.0/legalcode).

The license allows you to use, sell, share, modify and build on the files in almost any way you like - provided that you give credit/attribution, and that you share any changes that you make under the same open source license (see the [human readable version of the license](https://creativecommons.org/licenses/by-sa/3.0/) for a concise summary of the rights and obligations).

> **Note** Boards that are *derived directly* from Pixhawk schematic files (or reference boards) must be open sourced. They can't be commercially licensed as proprietary products.

Manufacturers can create (compatible) *fully independent products* by first generating fresh schematic files that have the same pin mapping/components as the FMU designs. Products that are based on independently created schematics are considered original works, and can be licensed as required.

Product names/brands can also be trademarked. Trademarked names may not be used without the permission of the owner.

> **Tip** *Pixhawk* is a trademark, and cannot be used in product names without permission.
