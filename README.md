# STM32 & C Mastery Plan

This repository documents my **8-week journey** to master **embedded systems programming using C and STM32 microcontrollers**. It also serves as a **professional portfolio** of the projects built during this plan.

---

##  Week 1 Projects

### 1️ Blinky (HAL & Bare-Metal)

This is the "**Hello, World!**" of embedded systems, designed to **set up the toolchain** and demonstrate basic hardware control.

####  Key Features

- **LED Pin Configuration:**
  - Configures the onboard LED pin (**PC13**) using both **STM32 HAL** and **bare-metal register manipulation**.

- **Blinking Logic:**
  - Implements a **500ms blink delay** using `HAL_Delay()`.

- **Memory-Mapped I/O:**
  - Demonstrates direct control of hardware by writing to the **GPIOC Output Data Register** (`GPIOC_ODR`) at address `0x40020814`.

---

### 2️ 8-Bit Bare-Metal LED Counter

This project demonstrates **low-level control** over an entire GPIO port by creating a **binary counter** with 8 LEDs.

####  Key Features

- **Bare-Metal Configuration:**
  - Configures pins **PA0 through PA7** as outputs by writing the value `0x00005555` to the `GPIOA_MODER` register.

- **Bare-Metal Control:**
  - Creates a binary counting effect from `0 to 255` by writing directly to the `GPIOA_ODR` register inside a `for` loop.

- **Learning Outcome:**
  - Demonstrates **mastery of GPIO architecture** and **bitwise operations** at the register level.

---

##  Technologies Used in Week 1

- **MCU:** STM32F401CCU6 (Black Pill)  
- **Language:** C  
- **IDE:** STM32CubeIDE  
- **Toolchain:** GCC for ARM  
- **Debugger:** ST-Link V2  

---

> This repository will continue to grow with more advanced embedded projects in the upcoming weeks.
