# Smart-_parking_tinkercad
The Smart Parking System is an Arduino-based project designed to automate the management of parking slots using servo motors and IR sensors. It features real-time monitoring of parking availability displayed on an LCD, enhancing efficiency and user interaction.




Smart Parking System

Project Overview 
The Smart Parking System is an Arduino-based project designed to automate and manage parking slots efficiently. Utilizing inexpensive and readily available hardware components, this system employs servo motors to control entry and exit gates, and infrared (IR) sensors to monitor the occupancy of parking slots. The state of each parking slot is displayed in real-time on an LCD display, providing a user-friendly interface for monitoring the status of the parking area.

Features
Automated Gate Control: Servo motors control the gates, which open automatically when a car arrives at the entrance or leaves through the exit.
Real-Time Slot Monitoring: IR sensors check the availability of parking slots and update the status on an LCD display. Each slot can show as 'Available' (A) or 'Not Available' (NA).
User-Friendly Display: A 16x2 LCD display shows the status of each parking slot, enhancing visibility and accessibility for users.
Scalable Design: The system is designed to be scalable, allowing for the addition of more parking slots and sensors with minimal adjustments to the code.

Components
Arduino Uno: Serves as the central controlling unit for the system.
Servo Motors (2x): Operate the entry and exit gates of the parking lot.
IR Sensors (4x): Detect the presence of vehicles in two parking slots and at the entry/exit points.
LiquidCrystal Display: A 16x2 LCD display used to show the status of each parking slot.
Wires and Breadboard: For connecting components and building the circuit.

How It Works
Setup: The system initializes by attaching the servo motors and setting the LCD display with a welcome message. It then displays the initial status of the parking slots.
Operation:
When a car approaches the entry gate, the corresponding IR sensor triggers, and the entry gate servo turns to open the gate.
As the car parks in a slot, the slot’s IR sensor detects the car, and the LCD updates the slot status to 'Not Available'.
When a car leaves the slot, the status updates back to 'Available', and when it passes through the exit, the exit gate opens.
Monitoring: The LCD continuously displays the real-time status of each parking slot, updating any changes based on sensor readings.

Code Structure
The code is organized into initialization in the setup() function, where hardware components are configured, and a loop() function, which runs continuously to check sensor states and update servo positions and the LCD display accordingly.

Installation
Connect the hardware according to the schematic provided in the repository.
Install the Arduino IDE and necessary libraries (Servo, LiquidCrystal).
Upload the Arduino sketch to the Arduino Uno board.
Power the Arduino and test the system functionality.

Future Enhancements
Implement web-based monitoring.
Add payment integration for commercial use.
Increase the number of parking slots and optimize space usage.
