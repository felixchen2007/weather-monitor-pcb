# Weather Monitor PCB — design notes

A complete embedded system, developed one iteration at a time.

## From breadboard to board

I developed the monitor through three iterations: a breadboard prototype, a PCB built around an ESP32 development board, and a fully integrated custom PCB designed in Altium Designer. Each iteration brought more of the system onto one board.

## Making the sensors talk

I wrote firmware to read temperature and humidity from a DHT11 and monitor power using an INA219. Debugging involved checking I²C addresses, communications, and pin assignments so the sensors and controller could work together.

## Turning measurements into information

A 240 × 240 ST7789 TFT display and a custom webpage present the measurements. The project connects hardware design, firmware, and a usable interface in a single system.

## Design focus

- ESP32 microcontroller
- Temperature & humidity sensing
- Solar power monitoring
- Display + web interface

[Back to the repository overview](../README.md)
