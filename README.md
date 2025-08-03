STM32 & C Mastery Plan
This repository documents my 8-week journey to master embedded systems programming using C and STM32 microcontrollers. It serves as my professional portfolio for the projects built during this plan.

Week 1 Projects
1. Blinky (HAL & Bare-Metal)
This is the "Hello, World!" of embedded systems, designed to set up the toolchain and demonstrate basic hardware control.

Key Features:

Configures the onboard LED pin (PC13) using both the STM32 HAL and direct bare-metal register manipulation.

Implements a 500ms blink delay using HAL_Delay().

Demonstrates understanding of memory-mapped I/O by finding and writing directly to the GPIOC ODR register at address 0x40020814.

2. 8-Bit Bare-Metal LED Counter
This project demonstrates low-level control over an entire GPIO port by creating a binary counter with 8 LEDs.

Key Features:

Bare-Metal Configuration: Configures pins PA0 through PA7 as outputs by writing a calculated value (0x00005555) directly to the GPIOA_MODER register.

Bare-Metal Control: Creates a binary counting effect from 0 to 255 by writing directly to the GPIOA_ODR register within a for loop.

This project proves a deep understanding of GPIO port architecture and bit manipulation at the register level.

Technologies Used in Week 1
MCU: STM32F401CCU6 (Black Pill)

Language: C

IDE: STM32CubeIDE

Toolchain: GCC for ARM

Debugger: ST-Link V2
