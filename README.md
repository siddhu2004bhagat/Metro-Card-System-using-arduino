RFID Metro Door Opening Gate

🚀 Project Overview

This project implements a Metro Door Opening System using an RFID module and Arduino. The system allows access control where a valid RFID card/tag triggers the opening of the metro gate (servo motors). Unauthorized access is denied, ensuring security and efficiency in metro stations.

🛠️ Components Used

Arduino Uno (or any compatible board)

RFID RC522 Module

Servo Motors (x2)

Buzzer (Optional for alerts)

LEDs (Optional for status indication)

Jumper Wires

12V Power Supply (if needed for servos)

🔌 Wiring Diagram

RFID RC522 Pin

Arduino Uno Pin

VCC

3.3V

GND

GND

RST

D9

SDA (SS)

D10

SCK

D13

MOSI

D11

MISO

D12

Servo Connections

Servo Motor Pin

Arduino Pin

Signal (PWM)

D5 & D6

VCC

5V

GND

GND

📜 Installation & Setup

Clone the repository

git clone https://github.com/yourusername/RFID-Metro-Door-Project.git
cd RFID-Metro-Door-Project

Install Required Libraries
Open Arduino IDE and install the following libraries from Library Manager (Sketch > Include Library > Manage Libraries):

MFRC522.h (for RFID module)

Servo.h (for controlling servo motors)

Upload the Code

Connect your Arduino to the PC.

Open the rfid_door.ino file.

Select the correct board and port.

Click Upload.

⚙️ How It Works

The RFID reader continuously scans for a card/tag.

If a valid card is detected (pre-registered UID), the servos move to open the door.

If an unrecognized card is detected, access is denied (a buzzer can be triggered as an alert).

After a short delay, the servos return to the closed position.

🎥 Demo Video

🚀 Watch Demo (Replace with actual link)

🛠️ Future Improvements

Add OLED Display for status updates.

Implement Cloud Logging for tracking entries.

Use IoT for remote access management.

📜 License

This project is open-source under the MIT License. Feel free to use and modify it for educational purposes.

Made with ❤️ by Your Name


