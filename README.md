# CAN Transmitter

## Overview
The **CAN Transmitter** project is designed to send vehicle telemetry-like data over a CAN (Controller Area Network) bus. It simulates data such as speed, RPM, fuel level, and temperature, which can be received by a corresponding CAN Receiver.

The project is built using STM32 microcontrollers and uses USB CDC to log transmitted messages to a PC.

## Features
- Sends CAN messages on multiple standard IDs:
  - **0x200**: Speed
  - **0x201**: RPM
  - **0x202**: Fuel Level
  - **0x203**: Temperature
- Simulates realistic changes in telemetry data.
- USB logging for easy debugging and monitoring.
- Configurable CAN message frequency and content.

## Hardware Requirements
- STM32 development board (e.g., STM32F407VGT6 series)
- CAN transceiver (if not on-board)
- USB cable for PC connection
- Optional LEDs for status/debugging

### CAN Pin Connections
- **CAN_TX**: Connect to the TX pin of the CAN transceiver.
- **CAN_RX**: Connect to the RX pin of the CAN transceiver.
- Ensure proper termination resistors (120Ω) on the CAN bus if necessary.

## Software Requirements
- STM32CubeIDE
- STM32 HAL libraries
- USB CDC stack

## Installation
1. Clone the repository:

   ```bash
   git clone https://github.com/codewithleo-helloworld/CAN_Transmitter.git
