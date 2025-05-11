# Ardunio-RFID-Gate-Parking
🚗 Arduino-Based Gate Parking System Using RFID
This project is an automated parking gate system using RFID and Arduino. Vehicles with registered RFID cards are granted access, and the gate opens automatically. It enhances parking security and efficiency by automating the vehicle entry process.
VIDEO LINK : https://www.linkedin.com/posts/karan-shivankar-858011282_arduino-autoamtion-teamkyzer-activity-7309258625850466304-ThUN?utm_source=social_share_send&utm_medium=member_desktop_web&rcm=ACoAAESzfIQBYqDUkZfbGyoSHtqAjCeZoc9pNcQ

📦 Project Overview
This system simulates a real-world gate entry mechanism commonly used in parking lots, offices, and residential complexes. The RFID reader detects an RFID tag, and upon successful identification, the Arduino controls a servo motor to open the gate.

🔧 Components Used
Component	Quantity
Arduino Uno	1
RFID Reader (RC522)	1
RFID Tags/Cards	1–2
Servo Motor	1
Jumper Wires	As needed
Breadboard	1
Buzzer (optional)	1
LED (optional)	1
Power Supply / USB	1

🔌 Circuit Diagram
(You can upload a diagram image here, or I can generate one for you—just let me know!)

Connections (RC522 to Arduino UNO):

SDA → D10

SCK → D13

MOSI → D11

MISO → D12

IRQ → Not Connected

GND → GND

RST → D9

3.3V → 3.3V

Servo Motor:

Signal → D6

VCC → 5V

GND → GND

💻 Code Explanation
The Arduino sketch does the following:

Initializes the RFID module and servo motor.

Continuously checks for RFID tags.

Compares the scanned UID with predefined UIDs.

If matched, the servo opens the gate.

After a short delay, the gate closes again.

Key Functions:
MFRC522 library for RFID communication.

Servo library to control the gate.

Delay used to simulate gate open time.

🚀 How to Use
Connect the hardware as per the diagram.

Upload the Arduino code to your Arduino Uno.

Power the system.

Place a registered RFID card near the reader.

The gate (servo motor) will open if the UID matches.

