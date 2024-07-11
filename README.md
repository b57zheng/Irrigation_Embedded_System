# Irrigation Embedded Control System

## Description
This project is an embedded control system designed for managing irrigation effectively. Utilizing a Nucleo F401RE board, this system integrates various sensors and actuators through a custom-designed PCB, enabling automated water distribution based on real-time environmental data.

## System Overview
- **MCU Controller**: Nucleo F401RE Development Board
- **Sensors**: Interfaces for US100 water depth sensor and other environmental parameters
- **PMW Motor Control**: Includes L9110 motor speed control for pumps and MG90S servo motor control for valves
- **Buffers**: Includes CD74HCT541 and CD74HC4050 for logic level translation
- **User Interface**: Input and indicator interfaces for real-time control and monitoring through UART protocol

## System Schematic
![image](https://github.com/b57zheng/Irrigation_Embedded_System/assets/98293562/716ed24c-8964-42d3-9bc7-f9799ea17960)

## PCB Layout
![image](https://github.com/b57zheng/Irrigation_Embedded_System/assets/98293562/4ec3f893-8ab0-410b-a109-c003f8dbbc2a)
![image](https://github.com/b57zheng/Irrigation_Embedded_System/assets/98293562/c79fdecf-29c5-4000-bb45-4394bec07f31)
![image](https://github.com/b57zheng/Irrigation_Embedded_System/assets/98293562/f74db943-f429-45e2-9c53-7241a2b4181b)

## Hardware and Software Requirements
- **Nucleo F401RE Board**
- **Custom PCB**
- **Sensors and Actuators as specified in the design**
- **Recommended IDE**: STM32Cube 1.13.2

## Installation
1. Assemble the hardware on the custom PCB following the schematic provided.
2. Flash the Nucleo board with the firmware included in the repository.
3. Connect all peripheral components as per the connection diagrams.

## Usage
### Setup Mode
- Reset the Nucleo board to enter the setup mode.
- Configure each zone and inlet by setting the PWM values through the terminal interface as detailed in the setup guide.

### Run Mode
- Start the system by setting the current wall clock time.
- The system operates automatically based on the preset schedules, adjusting the water distribution according to the sensor inputs.

## Contributing
Contributors are welcome to propose improvements to the system.
