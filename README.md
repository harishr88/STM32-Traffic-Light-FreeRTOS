# STM32 Traffic Light Controller with FreeRTOS

## Overview
A smart traffic light system built on STM32F103 Blue Pill using 
FreeRTOS demonstrating real-time embedded systems concepts.

## Hardware
- STM32F103C8T6 Blue Pill
- 3 LEDs (Green, Yellow, Red) on PA1, PA2, PA3
- Push button on PA0

## Features
- Traffic light sequence G(3s) → Y(1s) → R(3s) using FreeRTOS tasks
- Short press → Emergency mode (fast cycle)
- Long press  → Night mode (yellow blink only)
- Hardware interrupt via EXTI on button
- Semaphore from ISR to task
- Task suspend/resume for mode switching
- Watchdog timer for system reliability

## FreeRTOS Concepts Demonstrated
- Multiple tasks running concurrently
- Binary semaphore — ISR signals task
- Task suspend/resume
- Priority based scheduling
- osDelay for non-blocking timing

## Tools Used
- STM32CubeIDE
- STM32CubeMX
- FreeRTOS (CMSIS-RTOS v2)
- ST-Link V2 for flashing

## How to Run
1. Clone this repository
2. Open in STM32CubeIDE
3. Build and flash to Blue Pill
4. Connect LEDs to PA1, PA2, PA3 with 220 ohm resistors
5. Connect button to PA0 with pull-up

## Demo
[Add video link here after recording]
