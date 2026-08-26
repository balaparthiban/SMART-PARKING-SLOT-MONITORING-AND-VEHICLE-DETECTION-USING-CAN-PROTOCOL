Smart Parking Slot Monitoring and Vehicle Detection System using CAN Protocol

Overview

A 6-slot smart parking system developed using ARM7 LPC2129 microcontrollers and CAN communication. The system detects vehicle entry and exit using IR sensors, records time using RTC, displays parking information on an LCD, and controls the parking gate using a servo motor.

Hardware

* 3 × ARM7 LPC2129
* 2 × IR sensors
* RTC
* LCD
* Servo motor
* CAN transceiver/interface
* Power supply

Communication Protocols

* CAN – Communication between the three LPC2129 nodes
* I²C – Communication between LPC2129 and RTC
* UART – Debugging/serial communication

Working

* IR Sensor 1 detects vehicle entry.
* IR Sensor 2 detects vehicle exit.
* RTC provides the current date and time.
* Node 2 sends entry information using CAN ID 0x150.
* Node 2 sends exit information using CAN ID 0x151.
* Node 1 updates the available parking-slot count and displays the status on the LCD.
* Node 3 controls the parking gate using a servo motor.
* The system displays PARKING FULL when all 6 slots are occupied.

Features

* 6-slot parking management
* Automatic vehicle detection
* Entry and exit monitoring
* RTC-based time tracking
* CAN-based multi-node communication
* LCD parking-status display
* Automatic gate control

Technologies

ARM7 LPC2129 | Embedded C | CAN | I²C | UART | IR Sensor | RTC | LCD | Servo Motor

Applications

* Shopping malls
* Hospitals
* Airports
* Offices
* Smart-city parking systems
