# ESP32-POE-A
## Introduction:
ESP32-POE-A is a low-cost development kit for ESP32 with Active Power Over Ethernet support. The board uses LAN8720A chip for ethernet and CH340G USB-UART converter for communication with PC and programming.

## Features:

- ESP32-Wroom module.
- USB-C connector.
- 17 Pins are available.
- LAN8720A chip for Ethernet.
- Si3404 for POE.
- CH340G USB-UART converter.
- POE-LED, USER-Led(GPIO2).
- Reset button and User button(GPIO0).
- Accepts power through:
  - USB
  - External source (1.8V-5V)
  - Active POE

## Pinout and dimensions
![pinout](pictures/V1/pinout_ver1.png)

## Programming options:
Using vscode Platformio or Arduino IDE

## Uploading example project:
For example projects go to https://github.com/prokyber/ESP32-POE-A-PlatformIO-Example and https://github.com/prokyber/ESP32-POE-A-ArduinoIde-Example

## POE
The POE-Jumper should be on to supply 3.3V to ESP32 via POE.

## Important Notice
There is no galvanic isolation, so the board should not be connected to POE while programming. Disconnect POE jumper or use non-POE cable and supply power via USB.

## Schematics
Schematics can be found in HW/Vx/schematics
# Esp32-Stick-Boards-Docs
