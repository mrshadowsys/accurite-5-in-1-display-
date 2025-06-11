# AcuRite 5-in-1 Receiver with Arduino Nano

This project is an Arduino Nano-based receiver for decoding signals from an AcuRite 5-in-1 weather station. It uses a low-cost OOK (On-Off Keying) 433 MHz receiver module and displays weather data on a 16x2 character LCD.

## Features

- Decodes data from AcuRite 5-in-1 sensor suite
- Displays:
  - Temperature
  - Humidity
  - Wind speed
  - Wind direction
  - Rainfall
- Compatible with standard 433 MHz OOK receiver modules
- Compact and low power
- Uses standard 16x2 LCD (HD44780-compatible) with I2C or parallel interface

## Hardware Requirements

- Arduino Nano
- 433 MHz OOK receiver module (e.g., RXB6 or similar)
- 16x2 LCD display (with or without I2C backpack)
- Optional: Pull-up resistors for signal stability
- Breadboard and jumper wires

## Wiring

| Arduino Nano Pin | Connected To        |
|------------------|---------------------|
| D2               | Receiver Data Out   |
| A4 (SDA)         | LCD SDA (if I2C)    |
| A5 (SCL)         | LCD SCL (if I2C)    |
| 5V               | LCD VCC, Receiver VCC |
| GND              | LCD GND, Receiver GND |

> For non-I2C displays, connect RS, E, D4–D7 to any available digital pins and adjust the code accordingly.
