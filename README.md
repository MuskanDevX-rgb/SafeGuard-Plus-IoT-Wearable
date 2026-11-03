🛡️ SafeGuard+ – Smart IoT Wearable for Women's Safety

<p align="center">
[view SafeGuard Poster (pdf)](1.pdf)
</p>
<p align="center">
<img src="Images/2.jpeg" alt="SafeGuard+ Banner" width="100%">
</p>
<p align="center">
<img src="Images/3.jpeg" alt="SafeGuard+ Banner" width="100%">
</p>
<p align="center">
<img src="Images/4.jpeg" alt="SafeGuard+ Banner" width="100%">
</p>

<p align="center">
**A Standalone IoT-Based Women's Safety Wearable Using ESP32, GPS and GSM Technology**
</p>

📌 Project Overview

SafeGuard+ is a standalone IoT-based wearable safety device designed to provide emergency assistance through GPS tracking and GSM communication.

The system uses an ESP32 microcontroller integrated with a GPS module, GSM module, and motion sensor to provide emergency alerts and location tracking.

When the user presses the SOS button, the device sends an emergency SMS containing the user's current GPS location to registered emergency contacts and attempts to make emergency calls.

The system also includes geofencing functionality to detect movement beyond a predefined 5 km radius and experimental fall detection using an MPU6050 accelerometer and gyroscope.

🎯 Objectives
To develop a low-cost standalone wearable safety device.
To provide emergency alerts through SMS and calls.
To share real-time GPS location with registered emergency contacts.
To implement geofencing for location-based alerts.
To explore fall detection using the MPU6050 sensor.
To improve personal safety through embedded IoT technology.
✨ Key Features
SOS Emergency Alert: Sends an emergency SMS when the SOS button is pressed.
GPS Tracking: Retrieves the current geographical coordinates using the NEO-6M GPS module.
Location Sharing: Generates a Google Maps link and shares it through SMS.
Geofencing: Detects movement beyond a predefined 5 km radius.
Emergency Calling: Attempts to call configured emergency contacts.
Fall Detection: Uses the MPU6050 sensor for basic fall-event detection.
Standalone Operation: Works without requiring a smartphone application.
🛠️ Hardware & Prototype Overview
1. Components Overview

!SafeGuard+ Components Overview

Figure 1: Complete hardware breakdown including ESP32 development board, SIM800L GSM/GPRS module, NEO-6M GPS module, power management unit, and trigger switches.

2. Circuit Connections

!SafeGuard+ Circuit Diagram

Figure 2: Pin mapping and wiring connections between the ESP32 microcontroller, GPS module, GSM module, and power supply.

3. Hardware Assembly

!SafeGuard+ Hardware Assembly

Figure 3: Intermediate hardware integration showing compact module placement and wire routing prior to final enclosure.

4. Final Prototype

!SafeGuard+ Final Prototype

Figure 4: Fully assembled wearable SafeGuard+ device enclosed in a protective casing with accessible emergency alert controls.

🔩 Hardware Components
Component	Purpose
ESP32 Development Board	Main microcontroller
NEO-6M GPS Module	GPS location tracking
SIM800L GSM Module	SMS and emergency calls
MPU6050 Sensor	Fall detection
SOS Push Button	Manual emergency trigger
Li-Po Battery	Power supply
TP4056 Module	Battery charging
MT3608 Boost Converter	Voltage conversion
Jumper Wires	Circuit connections
Breadboard	Hardware prototyping
💻 Software & Technologies
Arduino IDE
Embedded C/C++
ESP32 Microcontroller
GPS Communication
GSM Communication
UART Communication
I2C Communication
TinyGPSPlus Library
⚙️ Working Principle
The ESP32 initializes the GPS, GSM, and MPU6050 modules.
The GPS module receives satellite signals and obtains the device's current location.
The first valid GPS location is stored as the geofence centre.
When the SOS button is pressed, the ESP32 generates an emergency alert.
An SMS containing the Google Maps location link is sent to registered emergency contacts.
The device attempts emergency calls to configured contacts.
If the device moves beyond the configured 5 km geofence radius, a location-based alert is triggered.
The MPU6050 continuously provides acceleration and gyroscope data for basic fall-event detection.
📂 Repository Structure
text
SafeGuard-Plus/
│
├── Code/
│   └── SafeGuard_Plus_Final.ino
│
├── Documentation/
│   ├── Project_Report.pdf
│   └── Research_Paper.pdf
│
├── Circuit_Diagram/
│   └── Circuit_Diagram.png
│
├── Images/
│   ├── SafeGuard_Banner.png
│   ├── Components.jpg
│   ├── Circuit_Connections.jpg
│   ├── Hardware_Assembly.jpg
│   └── Final_Prototype.jpg
│
├── Demo/
│   └── Demo_Link.txt
│
└── README.md

🚀 Setup & Installation
Prerequisites
Arduino IDE
ESP32 Board Package
TinyGPSPlus Library
Required hardware components
USB cable for programming
Installation Steps
Install the Arduino IDE.
Install the ESP32 board package through Boards Manager.
Install the TinyGPSPlus library through Library Manager.
Clone or download this repository.
Open Code/SafeGuard_Plus_Final.ino.
Configure the emergency contact numbers locally in the source code.
Connect all hardware components according to the circuit diagram.
Select the appropriate ESP32 board and COM port.
Upload the sketch to the ESP32.
Test GPS positioning, GSM communication, SOS alerts, geofencing, and fall detection.
🔔 Expected System Output
Emergency SMS with Google Maps location link.
Emergency call attempts to registered contacts.
Geofence-based location alerts.
Basic fall-event detection through MPU6050 sensor readings.
⚠️ Project Limitations
GPS positioning may be unavailable indoors or in areas with poor satellite reception.
GSM communication depends on compatible 2G network availability.
Fall detection is experimental and may generate false alerts.
Emergency SMS and calls depend on network coverage and stable module power.
The first valid GPS location may not always represent a safe or appropriate geofence centre.
🔮 Future Scope
Improved fall detection using sensor calibration and testing.
More reliable emergency alert confirmation.
Compact and comfortable wearable enclosure.
Improved battery backup and power management.
Integration with mobile applications.
Advanced location tracking and alert management.
📚 Project Information
Details	Description
Project Name	SafeGuard+
Domain	Internet of Things (IoT)
Platform	ESP32
Project Type	Standalone IoT Wearable Safety Device
Programming Language	Embedded C/C++
Communication	GPS and GSM
Development Environment	Arduino IDE
⚖️ Disclaimer

SafeGuard+ is an academic prototype developed for educational and research purposes.

It is not a replacement for verified emergency services or a guaranteed personal safety system. GPS accuracy, GSM network availability, battery performance, and sensor reliability may affect its operation.

Users should not depend exclusively on this prototype during emergencies.

👨‍💻 Project Repository

Explore the source code, hardware documentation, circuit diagrams, and prototype images in this repository.

SafeGuard+ – Smart IoT Wearable for Women's Safety

<p align="center">
*Technology for a safer tomorrow.*
</p>
