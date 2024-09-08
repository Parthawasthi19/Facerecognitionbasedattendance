# Face Recognition-Based Attendance System

## Overview
The Face Recognition-Based Attendance System is an AI-powered solution designed to automate and simplify the attendance process. Utilizing advanced machine learning techniques, particularly facial recognition, this project helps organizations or institutions streamline attendance management. By detecting and identifying faces in real-time, it marks attendance efficiently, reducing manual errors and ensuring accuracy.

## Components and Technologies
This system integrates several key components to deliver seamless functionality:
- **Face Detection & Recognition**: Detects human faces from video streams and compares them with pre-stored images for identification.
- **Database**: A centralized database for storing the facial data, names, and timestamps of attendance records.
- **User Interface**: A simple GUI allows for capturing and registering new faces, monitoring live attendance, and generating reports.
- **Real-time Processing**: Leverages computer vision to process and recognize faces in real time.

### Technologies Used:
- **OpenCV**: For real-time face detection and image processing.
- **Python**: The core programming language used for backend logic and machine learning integration.
- **dlib**: For facial feature detection and face recognition using machine learning models.
- **SQLite**: For storing and managing attendance records.
- **Tkinter**: To develop a user-friendly graphical interface.

## Features
- **Automated Attendance Marking**: Automatically registers attendance by recognizing the face of the individual.
- **Real-Time Face Detection**: Captures and recognizes faces from live video streams.
- **Database Management**: Stores attendance records in an SQLite database.
- **Report Generation**: Generates daily, weekly, or monthly attendance reports.
- **User-Friendly Interface**: Easy-to-use interface for capturing new faces and viewing attendance history.

## Installation

### Prerequisites
Ensure you have the following software and libraries installed:
- Python 3.x
- OpenCV
- dlib
- NumPy
- SQLite
- Tkinter (optional, for GUI)

### Steps to Install:
1. **Clone the repository**:
   ```bash
   git clone https://github.com/Parthawasthi19/Facerecognitionbasedattendance.git
   cd Facerecognitionbasedattendance
   ```

2. **Install required Python libraries**:
   ```bash
   pip install opencv-python dlib numpy
   ```

3. **Setup Database**:
   - Run the provided script to set up the SQLite database.
   ```bash
   python setup_db.py
   ```

4. **Run the Application**:
   To start the application, execute the following command:
   ```bash
   python main.py
   ```

## Usage
1. **Register New Users**: Capture images of the person whose attendance needs to be tracked and register them in the system.
2. **Start Attendance Session**: Use the live video feed to capture and mark attendance automatically when a registered person is recognized.
3. **Generate Reports**: View and export attendance reports for specified time periods.

## Conclusion
This Face Recognition-Based Attendance System is an effective and efficient solution for automating attendance management using facial recognition. With real-time processing, easy setup, and reliable performance, this project has practical applications in educational institutions, offices, and other organizational settings.

## Contact
For any questions, issues, or feedback regarding the Face Recognition-Based Attendance System, please

contact awasthiparth11@gmail.com.
