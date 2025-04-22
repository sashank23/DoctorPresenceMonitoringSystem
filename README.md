
# Doctor Presence Monitoring System

## Project Overview

The **Doctor Presence Monitoring System** is an advanced **contactless attendance tracking** solution designed for healthcare environments. By leveraging cutting-edge **face recognition technology**, this system automates attendance marking, making it ideal for hospitals, clinics, and medical institutions. The solution ensures real-time monitoring of doctors’ presence, offering a hygienic, efficient, and error-free method for tracking attendance.

This system eliminates the need for traditional time clocks, biometric scans, or physical attendance sheets, ensuring a seamless experience for both healthcare workers and administrators.

## Features

- **Real-Time Monitoring**: Detects doctor presence in real-time via a live webcam feed, instantly marking the doctor as "Present" or "Absent".
  
- **Face Recognition**: Utilizes pre-trained facial recognition models to identify registered doctors with high accuracy. Ensures that attendance is recorded automatically as soon as the doctor enters the frame.
  
- **Attendance Tracking**: Marks the doctor as "Present" immediately after face recognition and switches to "Absent" after a 10-second inactivity period (if the doctor leaves the frame).
  
- **Live Status Display**: The system displays real-time status updates on the doctor's presence. The status is color-coded:
  - **Green**: Present
  - **Red**: Absent
  
- **Touch-Free Interface**: Completely contactless, making it the perfect solution for maintaining hygiene and safety in a healthcare environment.
  
- **Real-Time Alerts**: The system can be integrated with notifications to alert administrators about absences or any discrepancies in attendance.

## Technologies Used

- **Python**: The core language used for implementing the logic behind the system.
  
- **OpenCV**: Handles video capturing and graphical user interface (GUI) rendering. OpenCV is used for real-time image processing tasks like face detection and recognition.
  
- **Face Recognition (dlib-based)**: A powerful library for face encoding, matching, and comparison. It uses pre-trained models to efficiently recognize doctors based on facial features.
  
- **NumPy & DateTime**: NumPy helps manage arrays of data (e.g., attendance logs), while DateTime is used for managing timestamps and the time period of inactivity.

## Setup & Installation

### Prerequisites

Before you begin, make sure you have Python 3.x installed. You will also need the following Python libraries:

- `opencv-python`: For video capture and GUI display.
- `face_recognition`: For facial recognition tasks.
- `numpy`: For array manipulation.
  
You can install these libraries via `pip`:

```bash
pip install opencv-python face_recognition numpy
```

### Running the System

1. **Clone the repository**:
   First, clone the project repository from GitHub:

   ```bash
   git clone https://github.com/YourUsername/Doctor-Presence-Monitoring.git
   ```

2. **Navigate to the project folder**:

   ```bash
   cd Doctor-Presence-Monitoring
   ```

3. **Run the Python script** to launch the system:

   ```bash
   python main.py
   ```

   The system will activate the webcam, begin face detection, and track attendance in real time.

4. **Monitor the real-time attendance**: The GUI will show the doctor’s name and status (Present or Absent) with color-coded feedback. The system will automatically update the status based on doctor presence or absence.

## Usage

Once the system is running:

- The camera will detect and recognize registered doctors via facial features.
- Each detected doctor's attendance will be marked as "Present".
- If no face is detected within 10 seconds, the status will be updated to "Absent".
- Admins and staff can view real-time attendance updates, which include:
  - **Doctor's Name**
  - **Presence Status** (Green for Present, Red for Absent)

## Future Enhancements

1. **Database Integration**: Store attendance logs in a centralized database for historical tracking, analysis, and reporting.
   
2. **Email & SMS Notifications**: Automatically send alerts to administrators or staff when a doctor is marked absent or when any discrepancies arise.

3. **Mobile Interface**: A mobile app interface can be developed to allow remote monitoring of attendance, particularly useful for administrators who need to manage multiple locations.

4. **Security Features**: Add advanced anti-spoofing techniques, such as **liveness detection**, to prevent unauthorized users from tricking the system with photos or videos.

5. **Offline Mode**: Implement offline functionality that can record attendance and sync later once the internet is restored.

## License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

