# ESP32-Stick
## Introduction:
ESP32-Stick is a line of low-cost development boards for ESP32 with Ethernet support. The boards use LAN8720A chip for ethernet and CH340G USB-UART converter for communication with PC and programming. ESP32-Stick-PoE-P provides passive Power-Over-Ethernet support(9-57V) and Esp32-Stick-PoE-A is capable of working with Active Power-Over-Ethernet.Programming is performed via USB connector.

## Features:

- ESP32-Wroom module.
- USB-C connector.
- 17 Pins are available.
- LAN8720A chip for Ethernet.
- LM2596HV for Passive POE(PoE-P).
- Si3404-A(PoE-A)
- CH340G USB-UART converter.
- USER-Led(GPIO2).
- Reset button and User button(GPIO0).
- Accepts power through:
  - USB
  - External source (3.3V-5V)
  - Passive POE(PoE-P)
  - Active POE(PoE-A)


## Pinout and dimensions
![Esp32-Stick-Eth pinout](/pictures/Esp32-Stick-PoE-P/pinout_ver2.png)

Dimensions are the same:
![Dimensions](/HW/Esp32-Stick-PoE-P/V1/PCB_ESP32-POE-P_ver.1_2022-12-31_dimensions.png)

## Programming options:
Using vscode Platformio or Arduino IDE

## Uploading example project:
For example projects go to https://github.com/allexoK/Esp32-Stick-Arduino-Examples , https://github.com/allexoK/Esp32-Stick-ESPHome-Examples and https://github.com/allexoK/Esp32-Stick-Platformio-Examples

## Important Notice
There is no galvanic isolation, so the board should not be connected to POE while programming. While programming use non-POE cable and supply power via USB.

## Schematics
Schematics can be found in HW/x/Vx/schematics

## On PoE compatibility
- Esp32-Stick-PoE-A was tested to work with TR60A-POE-L(48V) from Microelectronics tech INC. and POE15F(48V) from Tenda.
- Esp32-Stick-PoE-P was tested to work with TR60A-POE-L(48V), POE15F(48V) , UBI-POE-24-1(24V), GP-B240-100(24V),  GP-240-050(24V), GP-A240-050,  APOE24V-1, UBI-POE-24-5
- One user reported problems with USW-Pro-24-POE (400W) switch. Perhaps some PoE incompatibility issues.

## Troubleshooting Esp32-Stick-Boards
1. I am powering Esp32-Stick-PoE-A with PoE adapter and the power led is off:
- Are you sure you are using 48V PoE adapter?
- Are you using type B power adapter?(The power must be supplied via pins 4,5 and 7,8)?
- Have you tried different adapter?
- Try using shorter Ethernet cable, did it help?

2. I have a network connection problems:
- Try using shorter Ethernet cable, did it help?

