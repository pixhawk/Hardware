# Reference Hardware for PX4 Sapog

[![Join the chat at https://gitter.im/Zubax/general](https://img.shields.io/badge/GITTER-join%20chat-green.svg)](https://gitter.im/Zubax/general)

This directory contains the reference hardware design for
[PX4 Sapog](https://kb.zubax.com/x/cYAh) - an advanced open source ESC firmware.

This specific design is intended as an application note;
the main knowledge to gather from this design is the pinout of the MCU and its immediate connections.
The design is implemented in Eagle, version 7 or newer is required.

## Resources

* **[HOMEPAGE](https://kb.zubax.com/x/cYAh)**
* **[SUPPORT & FEEDBACK](https://forum.zubax.com/)**
* **[FIRMWARE ON GITHUB](https://github.com/PX4/sapog)**

## Design guidelines

1. When choosing the power transistors, keep their dynamic characteristics in mind:
the switching time must be under 50 nanoseconds.
Sapog employs somewhat unorthodox methods of state estimation which require a high-speed inverter.
2. The RC filters in the phase voltage feedback circuits should be designed so that their cutoff frequency
is around 19 kHz and the output impedance does not exceed 8 kohm.
3. Unless your maximum supply voltage exceeds 25 V (6S), do not change the DC link voltage measurement divider.

## License

The design is distributed under the terms of the
Creative Commons Attribution-ShareAlike 3.0 Unported license (CC BY-SA 3.0).
