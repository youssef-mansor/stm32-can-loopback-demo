# STM32 CAN Loopback Demo

A minimal example demonstrating CAN communication on the STM32L432KC using **loopback mode**.  
It covers CAN peripheral configuration with CubeMX, frame transmission, filtering, and interrupt-based reception using HAL.

## Features
- STM32L432KC HAL-based CAN setup
- Loopback mode for internal testing (no external transceivers required)
- Standard 11-bit identifier support
- Interrupt-driven message reception
- Configurable CAN frame data

## Files
- `CAN.ioc` – CubeMX project configuration
- `Core/` – Source code (main, HAL initialization, interrupt handling)
- `Drivers/` – HAL and CMSIS drivers
- `STM32L432KCUX_FLASH.ld` – Linker script

## Usage
1. Open `CAN.ioc` in STM32CubeMX to generate project files.
2. Build and flash the project using STM32CubeIDE.
3. Observe loopback CAN messages using the debugger or CAN monitoring tools.

## Notes
- Only loopback mode is implemented; no external CAN transceivers are required.
- The project is meant as a learning/demo example for STM32 CAN.

