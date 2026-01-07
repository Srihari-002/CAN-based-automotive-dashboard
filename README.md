# CAN-based-automotive-dashboard
🚗 CAN-Based Automotive Dashboard (3-Node System)
📌 Project Overview

This project implements a CAN (Controller Area Network) based automotive dashboard using three PIC microcontroller boards.
Each board acts as an independent ECU and communicates over the CAN bus to simulate a real vehicle instrument cluster.

🎯 Objective

To understand multi-node CAN communication

To simulate real automotive ECU behavior

To gain hands-on experience in embedded firmware and hardware integration

⚙️ System Architecture
🔹 Node 1 – Dashboard ECU

Receives data from other ECUs via CAN

Displays speed, RPM, and gear position on SSD/LCD

Controls dashboard indicators

Uses interrupt-driven CAN reception

🔹 Node 2 – Speed & Gear ECU

Generates speed and gear data (ADC / input based)

Packs data into CAN frames

Transmits data periodically to dashboard ECU

🔹 Node 3 – RPM & Indicator ECU

Generates RPM and indicator status

Sends RPM and indicator data over CAN

Simulates engine-related parameters

🧠 Key Features

Three-node CAN network

Standard CAN identifiers for different ECUs

Separate CAN messages for speed, gear, RPM, and indicators

Interrupt-based CAN communication

Real-time dashboard updates

🛠️ Technologies Used

PIC Microcontrollers

Embedded C

CAN Protocol

MPLAB X IDE

XC8 Compiler

ADC, GPIO, Timers

🚧 Challenges Faced

CAN message collision and arbitration understanding

Incorrect mask and filter configuration across multiple nodes

Synchronization issues between speed and RPM updates

Display flickering due to blocking delays

CAN bus instability without proper 120Ω termination resistors

📚 Learnings

Multi-ECU communication using CAN

CAN arbitration and priority handling

Importance of message IDs, filters, and timing

Real-time embedded system design

Debugging complex embedded systems

🔮 Future Improvements

Add fuel level and temperature ECUs

Implement CAN error frames handling

Add graphical dashboard display

Support data logging and diagnostics

👤 Author

Sri Hari
Embedded Systems Enthusiast
