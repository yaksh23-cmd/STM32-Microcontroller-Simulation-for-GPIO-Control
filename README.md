# STM32-Microcontroller-Simulation-for-GPIO-Control

This project demonstrates a basic **LED blinking** application using the **STM32F103C6 microcontroller**.  
The code is written and compiled in **STM32CubeIDE**, and the hardware simulation is done in **Proteus**.

---

## 📌 Project Overview
- **Microcontroller**: STM32F103C6 (ARM Cortex-M3, Blue Pill)  
- **IDE**: STM32CubeIDE  
- **Firmware**: STM32Cube HAL drivers  
- **Simulator**: Proteus 8 Professional  
- **Functionality**: The LED toggles ON/OFF at a fixed delay, showcasing GPIO output control.

---

## 🛠️ How It Works
1. The GPIO pin connected to the LED is configured as **output push-pull** in CubeIDE.  
2. A simple **delay loop / HAL_Delay()** is used to blink the LED at regular intervals.  
3. The compiled `.elf/.hex` file is loaded into the STM32F103C6 inside Proteus.  
4. The Proteus circuit includes:
   - STM32F103C6 microcontroller  
   - One LED connected to a GPIO pin with resistor  
   - Virtual ground and Vcc connections  

---
<img width="1024" height="775" alt="image" src="https://github.com/user-attachments/assets/cabdae7e-d9f4-4bc1-8d71-6bf92f2062f3" />


## ▶️ Running the Project
### 1. In STM32CubeIDE
- Open the project `.ioc` file.  
- Build the project (`Project → Build`).  
- The **.elf/.hex** file will be generated inside the `Debug/` or `Release/` folder.  

### 2. In Proteus
- Place the **STM32F103C6 microcontroller** in the schematic.  
- Connect an LED (with resistor) to the configured GPIO pin.  
- Load the generated `.hex` file into the MCU in Proteus.  
- Run the simulation → the LED should blink.  

---

