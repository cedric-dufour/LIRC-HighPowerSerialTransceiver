LIRC High-Power Serial Transceiver
==================================

This electronics project spawned from my need to blast Philips RC6 infrared
codes across my entire living room and remote control my existing Feller
Zeptrion [1] (house control) electric installation, with the help of the Linux
Infrared Remote Control (LIRC) [2].

Unfortunately, my existing USB dongle would not transmit RC6 codes while my
spare serial transmitter would lack the power to blast IR accross the entire
room.

I thus designed this High-Power Serial Transceiver with the following key
points in mind:

 1. high-power IR transmission, using an external power source such as the
    RS-232 12-volt "Power-over-System" provided by some card (e.g. Exsys
    44092-2 [3]) or using a 9-volt battery

 2. versatile IR reception, compatible with both 36/38kHz and 56kHz remotes

 3. indicator LED to monitor IR reception (and transmission)

 4. do-it-yourself using "off-the-shelf" standard components [4]

starting with the designs proposed by LIRC and its contributors:

   http://www.lirc.org/transmitters.html

   http://www.lirc.org/receivers.html

and using this opportunity to over-design some of the components, such as to
protect the high-power LEDs to be driven out of specifications by the full
range of potential RS-232 signals/voltages (using a high-pass input filter
and a two-transistors constant current source).

   ![Overview Image](/LIRC-HighPowerSerialTransceiver.jpg)


Provided files are:

 - KiCAD/Eeeschema schematic (and corresponding PDF plot)

 - KiCAD/PCBnew layout (and corresponding SVG export)

Please bear with me that the provided PCB layout is targeted towards 2.54mm-pad
rapid prototype boards rather than actual PCB manufacturing.


Enjoy!


References:

[1] https://www.feller.ch/de/Produktangebot/Licht-und-Storensteuerungssystem/Licht-Storensteuerung-zeptrion

[2] http://www.lirc.org

[3] http://www.exsys.de/index.php?page=product&info=202

[4] http://farnell.com

