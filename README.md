
### Face Recognition-Based Attendance System
#### Overview
The Face Recognition-Based Attendance System is an AI-powered solution designed to automate and simplify the attendance process. By leveraging advanced machine learning techniques, particularly facial recognition, this project helps organizations or institutions streamline attendance management. It detects and identifies faces in real-time, efficiently marking attendance, reducing manual errors, and ensuring accuracy.

In this version, Intel's **oneAPI** technologies, including **oneDAL** (Data Analytics Library) and **oneDNN** (Deep Neural Network Library), have been integrated to optimize the performance of machine learning tasks and facial recognition processes, especially for large-scale datasets.

---

### Components and Technologies

This system integrates several key components for optimized performance:

- **Face Detection & Recognition**: Detects human faces from video streams and compares them with pre-stored images for identification.
- **Database**: Centralized storage for facial data, names, and timestamps of attendance records.
- **User Interface**: A simple GUI allows for capturing and registering new faces, monitoring live attendance, and generating reports.
- **Real-time Processing**: Leverages computer vision and machine learning models optimized using oneAPI for efficient face recognition in real-time.

---

### Technologies Used

- **OpenCV**: For real-time face detection and image processing.
- **Python**: Core programming language for backend logic and machine learning integration.
- **dlib**: For facial feature detection and face recognition using machine learning models.
- **Intel oneDAL**: For accelerating data processing and machine learning operations like training and inference.
- **Intel oneDNN**: Optimizes the deep learning computations involved in facial recognition.
- **Intel oneAPI**: Provides a cross-architecture development framework to optimize workloads.
- **SQLite**: For storing and managing attendance records.
- **Tkinter**: To develop a user-friendly graphical interface.
  
Tested on **Intel Developer Cloud**, leveraging Intel's optimized hardware infrastructure.

---

### Features

- **Automated Attendance Marking**: Automatically registers attendance by recognizing faces.
- **Real-Time Face Detection**: Uses Intel's oneDNN and oneDAL to process large datasets with optimized performance.
- **Database Management**: Stores attendance records in an SQLite database.
- **Report Generation**: Generates daily, weekly, or monthly attendance reports.
- **User-Friendly Interface**: Easy-to-use interface for registering new faces and viewing attendance history.

---

### Installation

#### Prerequisites
Ensure you have the following software and libraries installed:

- Python 3.x
- OpenCV
- dlib
- NumPy
- SQLite
- Intel oneDAL, oneDNN, oneAPI Toolkit
- Tkinter (optional, for GUI)

#### Steps to Install:

1. Clone the repository:

   ```bash
   git clone https://github.com/Parthawasthi19/Facerecognitionbasedattendance.git
   cd Facerecognitionbasedattendance
   ```

2. Install required Python libraries:

   ```bash
   pip install opencv-python dlib numpy
   ```

3. Install Intel oneAPI components (oneDAL, oneDNN):

   ```bash
   # Install the oneAPI Base Toolkit and AI Analytics Toolkit from Intel's website
   # Follow the instructions to install oneDAL, oneDNN, and the necessary libraries.
   ```

4. Setup the SQLite Database:

   ```bash
   python setup_db.py
   ```

5. Run the Application:

   ```bash
   python main.py
   ```

---

### Usage

1. **Register New Users**: Capture images of the individuals whose attendance will be tracked and register them in the system.
2. **Start Attendance Session**: Use the live video feed to automatically capture and mark attendance when a registered face is recognized.
3. **Generate Reports**: View and export attendance reports for specified time periods.

---

### Integration with oneAPI, oneDAL, and oneDNN

This project utilizes Intel's oneAPI, oneDAL, and oneDNN for high-performance processing. By integrating oneDAL, facial recognition models are trained and optimized more efficiently. oneDNN accelerates deep learning computations in facial recognition tasks, ensuring that the system performs well even with larger datasets.

Tested on **Intel Developer Cloud**, ensuring scalability and performance across different hardware architectures.

---

### Conclusion

The Face Recognition-Based Attendance System provides an efficient and scalable solution for automating attendance management using facial recognition. With Intel oneAPI, oneDAL, and oneDNN integration, this project offers enhanced performance, making it suitable for use in educational institutions, offices, and other organizational settings.

---

### Contact

For any questions, issues, or feedback regarding the Face Recognition-Based Attendance System, please contact:

- **Email**: awasthiparth11@gmail.com
