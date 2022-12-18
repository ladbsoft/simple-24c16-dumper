# Simple-24c16-dumper
Very simple Arduino based 24c16 EEPROM programmer, based on [P-Find/arduino-24c16](https://github.com/P-Find/arduino-24c16)

## Pin connections
This connections are for the x24c16p from Xicor. Other variations of the 24c16 should be compatible, but cross reference the datasheet of your exact model before blaming me ;)

|Arduino|24c16|Comments|
|-------|-----|--------|
|SCL|SCL|Clock|
|SDA|SDA|Data|
|GND|A0|Address 0|
|GND|A1|Address 1|
|GND|A2|Address 2|
|GND|TEST (MODE/WC)|Mode/Write control|
|GND|GND|Ground|
|+5V|Vcc|Power|

## Instructions
- Upload sketch to an Arduino (Uno, Nano, Mega...)
- Connect using serial monitor
- Send a `c` to clear the chip, or an `s` to read it. Read data will be presented as hex in the serial console.
