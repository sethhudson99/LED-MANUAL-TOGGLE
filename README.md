# LED-MANUAL-TOGGLE
Bare metal STM32 GPIO project using register-level programming to read a digital input on PA0 (jumper wire) and control the onboard LED on PA5 without HAL libraries.

A simple embedded C project demonstrating direct register manipulation on an STM32F4 microcontroller without using HAL libraries. The program reads the logic level on GPIO pin PA0 and controls an LED connected to PA5.

## Features

- Bare-metal programming using memory-mapped registers
- No HAL or driver libraries
- Direct configuration of GPIOA registers
- Reads digital input on PA0
- Controls LED output on PA5
- Demonstrates bit masking and bitwise operations

## Hardware

- STM32 Nucleo-F446RE
- Onboard LED (PA5)
- Jumper wire used to apply a HIGH signal to PA0

## Program Operation

1. Enable the GPIOA peripheral clock.
2. Configure PA5 as an output.
3. Leave PA0 configured as an input.
4. Continuously read the state of PA0.
5. When PA0 is HIGH, turn the LED on.
6. When PA0 is LOW, turn the LED off.

## Concepts Demonstrated

- Memory-mapped I/O
- Pointer dereferencing
- GPIO configuration
- Register-level programming
- Bit masking
- Bitwise operations
- Polling-based input handling
- Embedded C programming

## Future Improvements

- Add a push button with pull-up/pull-down resistor
- Implement software debouncing
- Toggle the LED on each button press
- Use external interrupts (EXTI)
- Create reusable GPIO driver functions
- Replace hard-coded addresses with symbolic macros

## Tools Used

- STM32CubeIDE
- Embedded C
- STM32F446RE
- ARM Cortex-M4

## Learning Objectives

This project was created to understand how GPIO peripherals are controlled through memory-mapped registers and how digital inputs and outputs are manipulated at the hardware level without using abstraction libraries.
