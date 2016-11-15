Hardware
========

[![Join the chat at https://gitter.im/PX4/Hardware](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/PX4/Hardware?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

PX4 Hardware designs

Website at: http://pixhawk.org

PX4 is an open hardware design, following the OSHW 1.1 definition licensed under the Creative Commons Attribution-ShareAlike 3.0 Unported (CC BY-SA 3.0) license.

Pull requests for relevant fixes are very welcome.

Pixhawk v1 Hardware
===================

FMUv1 & FMUv2 boards

Design files are EAGLE CAD files (can be viewed with the free version)
www.cadsoftusa.com/

And BOM management is performed using Bob Starr's BOM-EX plugin:
http://www.bobstarr.net/pages/downloads.html

Pixhawk v2 Hardware
===================

FMUv3 board (and IMUv3 + PSMv3 support components)

The Pixhawk v2 Hardware is the result of a collaboration of the open hardware development community and 3D Robotics and has been designed in Altium.

MindPX V2 Hardware
===================
http://www.mindpx.net

MindPX V2.8 board

Product brief:
http://www.mindpx.net/assets/accessories/brochure.pdf

Hardware specification:
http://www.mindpx.net/assets/accessories/Specification_MindPX.pdf

User manual:
http://www.mindpx.net/assets/accessories/UserGuide_MindPX.pdf

Key features of v2.8:

1. 8 main PWM outputs + 8 aux PWM outputs
2. Dual-redundancy IMU components (onboard HMC5883L compass)
3. Support PPM/SBUS/SPEKTRUM DSM/Satellite RC input
4. Support FrSky/Wifi telemetry
5. One extra I2C port (so can support external compass and px4flow simultaneously)
6. Secondary USB port  for companion computer (converted from UART2 using onboard CP2104)
7. nrf/SPI port for SPI devices
8. exposed SWD debug port
9. Built-in vibration dampening for isolated IMU, support hard mount on air frames.
10. LTC2875 as CAN controller (+/- 60V overvoltage fault protection)

MindRacer V1.2 board (Hardware version: v1.2)

Key features of v1.2:
1. 35 x 35mm (30.5 mm mounting holes) ultra mini size, weighs about 6g
2. STM32F427 as processor
3. 6 main PWM outputs
4. onboard MPU6500 & HMC5883L
5. dual 2x7 stackable header pins for I/O port replication/expansion
6. optional IMU isolation mounting support
7. Support PPM/SBUS/SPEKTRUM DSM/Satellite RC input
8. Support FrSky/Wifi telemetry
9.  onboard RTC battery and TF card slot
10. DroneCode standard connectors

Note: MindPX v2.8 & MindRacer v1.2 share same firmware.

[Sapog ESC](https://github.com/PX4/sapog) Hardware
==================================================

The directory `sapog_reference_hardware` contains the reference hardware design for the
Sapog ESC firmware. Refer to its README.md for more info.

Creative Commons License Disclaimer
===================================

UNLESS OTHERWISE MUTUALLY AGREED TO BY THE PARTIES IN WRITING, LICENSOR OFFERS THE WORK AS-IS AND MAKES NO REPRESENTATIONS OR WARRANTIES OF ANY KIND CONCERNING THE WORK, EXPRESS, IMPLIED, STATUTORY OR OTHERWISE, INCLUDING, WITHOUT LIMITATION, WARRANTIES OF TITLE, MERCHANTIBILITY, FITNESS FOR A PARTICULAR PURPOSE, NONINFRINGEMENT, OR THE ABSENCE OF LATENT OR OTHER DEFECTS, ACCURACY, OR THE PRESENCE OF ABSENCE OF ERRORS, WHETHER OR NOT DISCOVERABLE. SOME JURISDICTIONS DO NOT ALLOW THE EXCLUSION OF IMPLIED WARRANTIES, SO SUCH EXCLUSION MAY NOT APPLY TO YOU.
EXCEPT TO THE EXTENT REQUIRED BY APPLICABLE LAW, IN NO EVENT WILL LICENSOR BE LIABLE TO YOU ON ANY LEGAL THEORY FOR ANY SPECIAL, INCIDENTAL, CONSEQUENTIAL, PUNITIVE OR EXEMPLARY DAMAGES ARISING OUT OF THIS LICENSE OR THE USE OF THE WORK, EVEN IF LICENSOR HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.

http://creativecommons.org/licenses/by-sa/3.0/
