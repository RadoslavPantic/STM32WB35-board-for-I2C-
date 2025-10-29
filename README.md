# STM32WB35 Custom Development Board

Custom development board based on STM32WB35 wireless microcontroller, designed for I2C sensor applications and environmental monitoring systems.

## Hardware Overview

This board implements a complete STM32WB35 development platform with focus on I2C sensor integration, particularly for Sensirion environmental sensors.

## Key Features

### Microcontroller
- STM32WB35CCU6 Arm Cortex-M4 core with Bluetooth 5.0 and 802.15.4
- 512KB Flash, 128KB SRAM
- Operating frequency up to 64MHz

### Power Management
- USB-C power input with 5V operation
- Li-Po battery support with charging circuit
- Multiple regulated outputs: 3.3V I/O, 1.8V core
- Power sequencing and brown-out protection

### Interfaces
- USB 2.0 full-speed with Type-C connector for programming and communication
- Dedicated I2C connector for sensor modules
- SWD debug interface
- GPIO breakout headers

### Protection Circuits
- ESD protection on all external interfaces
- Button debouncing circuits
- Manual reset circuit

## Hardware Specifications

### Power Supply
- Input voltage range: 3.7V to 5.5V
- USB-C: 5V ±5%
- Battery: 3.7V Li-Po
- Maximum current: 500mA

### Clock System
- Main crystal: 32MHz ±10ppm
- RTC crystal: 32.768kHz ±20ppm
- Internal RC oscillators available

### I2C Interface
- Standard mode (100kHz) and fast mode (400kHz)
- 3.3V logic levels
- Pull-up resistors included

## Pin Configuration

### I2C Sensor Connector (J1)
Pin 1: VCC_3V3  (Sensor power)
Pin 2: GND      (Ground)
Pin 3: I2C1_SDA (Data line)
Pin 4: I2C1_SCL (Clock line)

### Debug Interface (J2)
Pin 1: VDD_3V3
Pin 2: SWDIO
Pin 3: GND
Pin 4: SWCLK
Pin 5: NRST

## Repository Structure
