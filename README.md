# I^2C Scanner

(https://playground.arduino.cc/Main/I2cScanner/)

This very simple sketch scans the $I^2C$-bus for devices. If a device is found, it is reported to the Arduino serial monitor.

This sketch is the first step to get the $I^2C$ communication working.

The sketch shows the 7-bit addresses of the found devices as hexadecimal values. That value can be used for the "Wire.begin" function which uses the 7-bit address. Some datasheets use the 8-bit address and some example sketches use decimal addresses.

This sketch tests the standard 7-bit addresses. Devices with higher bit address might not be seen properly.


## Sketch

Open a new sketch and copy the sketch below into it. Upload it to the Arduino and open the serial monitor. Every found device on the I^2^C-bus is reported.

You can change the wires, and plug-in I^2^C devices while the i2c_scanner is running.


## Revision history

Version 1
This program (or code that looks like it) can be found in many places. For example on the Arduino.cc forum. The original author is not know.

Version 2, June 2012.
Using Arduino 1.0.1 by Arduino.cc user Krodal.
Adapted to be as simple as possible.

Version 3, February 26, 2013.
by louarnold.

Version 4, March 3, 2013.
Using Arduino 1.0.3 by Arduino.cc user Krodal.
Changes by louarnold removed. Scanning addresses changed from 0...127 to 1...119, according to the i2c scanner by Nick Gammon (https://www.gammon.com.au/forum/?id=10896).

Version 5, March 28, 2013.
As version 4, but address scans now to 127. A sensor seems to use address 120.

Version 6, November 27, 2015.
Added waiting for the Leonardo serial communication.

