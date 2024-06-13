# Embedded System Control with STM32 - Activate/Deactivate LED

## Overview
This project is an extension of coursework in Embedded C programming, focusing on direct manipulation of hardware registers within the STM32F407 microcontroller to control GPIO peripherals for LED activation.

## Key Features
- **Clock Activation**: Ensures power is supplied to GPIOD and GPIOA peripherals.
- **GPIO Configuration**: Sets specific GPIOD pins to output mode to drive LEDs and configures GPIOA pins for input to detect external voltage.
- **Dynamic LED Control**: LEDs are controlled based on the input pin status from GPIOA.

## Project Structure
- `main.c`: Implements the core functionality for configuring GPIO pins and controlling LEDs based on external input.

## Hardware and Tools
- **Microcontroller**: STM32F407
- **IDE**: STM32CubeIDE

## Setup and Run
1. Open the project in STM32CubeIDE.
2. Connect the STM32F407 development board.
3. Compile the code and flash it to the microcontroller.
4. Operate the input switches or sensors to observe LED behavior.
   
## Additional Setup Instructions
- **Voltage Activation for GPIOA Pin 0**: To allow voltage to pass to pin 0, connect a jumper wire from pin 0 to the VDD pin. This will trigger the LEDs.

## Detailed Operation
- **Clock Initialization**: Clocks for GPIOD and GPIOA are enabled to allow data and voltage passage.
- **Mode Configuration**:
  - GPIOD pins 12 to 15 are set to output mode to control LEDs.
  - GPIOA pin 0 is set to input mode to read sensor or switch signals.

