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

MindPX V2 board (Hardware version:   v2.2)
http://www.mindpx.net

Product brief:
http://www.mindpx.net/assets/accessories/brochure.pdf

Hardware specification:
http://www.mindpx.net/assets/accessories/Specification_MindPX.pdf

User manual:
http://www.mindpx.net/assets/accessories/UserGuide_MindPX.pdf

Revisions against Pixhawk:

1. 6 PWM distance sensors inputs
2. 1 extra parallel I2C port (so can support external compass and px4flow simultaneously)
3. Secondary USB port  for companion computer (converted from UART2 using onboard CP2104)
4. exposed SWD debug port
5. Built-in vibration dampening, support hard mount on air frames.
6. removed in v2.2:
        • Spektrum DSM / DSM2 / DSM-X® Satellite compatible input
        • Futaba S.BUS® compatible input and output
        • auxiliary outputs
        • safety switch (moved to power distribution board as eSwitch)

Note: MindPX v2.2 supports maximum 6 direct PWM outputs.


Creative Commons License Disclaimer
===================================

UNLESS OTHERWISE MUTUALLY AGREED TO BY THE PARTIES IN WRITING, LICENSOR OFFERS THE WORK AS-IS AND MAKES NO REPRESENTATIONS OR WARRANTIES OF ANY KIND CONCERNING THE WORK, EXPRESS, IMPLIED, STATUTORY OR OTHERWISE, INCLUDING, WITHOUT LIMITATION, WARRANTIES OF TITLE, MERCHANTIBILITY, FITNESS FOR A PARTICULAR PURPOSE, NONINFRINGEMENT, OR THE ABSENCE OF LATENT OR OTHER DEFECTS, ACCURACY, OR THE PRESENCE OF ABSENCE OF ERRORS, WHETHER OR NOT DISCOVERABLE. SOME JURISDICTIONS DO NOT ALLOW THE EXCLUSION OF IMPLIED WARRANTIES, SO SUCH EXCLUSION MAY NOT APPLY TO YOU.
EXCEPT TO THE EXTENT REQUIRED BY APPLICABLE LAW, IN NO EVENT WILL LICENSOR BE LIABLE TO YOU ON ANY LEGAL THEORY FOR ANY SPECIAL, INCIDENTAL, CONSEQUENTIAL, PUNITIVE OR EXEMPLARY DAMAGES ARISING OUT OF THIS LICENSE OR THE USE OF THE WORK, EVEN IF LICENSOR HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.

http://creativecommons.org/licenses/by-sa/3.0/
