Doctor Presence Monitoring System
Project Overview
The Doctor Presence Monitoring System is a contactless attendance tracking solution for healthcare environments. It uses face recognition technology to automate the attendance marking process. This system helps in tracking the presence of doctors in real-time and offers a hygienic, efficient, and error-free way of attendance monitoring.

Features
Real-Time Monitoring: Detects doctor presence in real-time via webcam feed.

Face Recognition: Utilizes pre-trained face data for accurate doctor identification.

Attendance Tracking: Marks doctors as "Present" upon recognition and "Absent" after 10 seconds of inactivity.

Live Status Display: Displays real-time status updates on doctor presence with color-coded feedback (Green for Present, Red for Absent).

Touch-Free Interface: Promotes hygienic operation, ideal for medical environments.

Technologies Used
Python: Core programming logic.

OpenCV: For video capture and GUI display.

Face Recognition (dlib-based): For encoding and comparing facial features.

NumPy & DateTime: For time management and array operations.

Setup & Installation
Prerequisites
Python 3.x

Required Python libraries:

opencv-python

face_recognition

numpy

You can install these libraries using pip:

bash
Copy
Edit
pip install opencv-python face_recognition numpy
Running the System
Clone this repository to your local machine:

bash
Copy
Edit
git clone https://github.com/YourUsername/Doctor-Presence-Monitoring.git
Navigate to the project folder:

bash
Copy
Edit
cd Doctor-Presence-Monitoring
Run the Python script to start the system:

bash
Copy
Edit
python main.py
The system will start detecting faces from the webcam feed and track attendance based on real-time recognition.

Usage
The system will automatically detect and recognize registered doctors via their facial features.

The attendance will be displayed live on the interface with the doctor's name and status (Present or Absent).

The system updates the status to "Absent" if no face is detected for more than 10 seconds.

Future Enhancements
Database Integration: Integrate with a database for storing historical attendance logs.

Email & SMS Notifications: Notify administrators or staff of any absences.

Mobile Interface: Develop a mobile application for monitoring doctor attendance remotely.

Security Features: Add anti-spoofing mechanisms like liveness detection to improve security.

License
This project is licensed under the MIT License - see the LICENSE file for details.
