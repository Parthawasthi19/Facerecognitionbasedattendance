# 🎯 Facial Recognition-Based Attendance System

A smart attendance system using facial recognition built with **Flask**, **OpenCV**, and **scikit-learn**. It captures faces through a webcam, recognizes registered individuals using a trained KNN model, and logs attendance in real time.

---

## 📌 Features

- 🧑‍🎓 Add and manage user faces
- 🎥 Real-time face detection via webcam
- 🧠 Trained KNN model for face recognition
- 🗓️ Automatically records date and time of attendance
- 📁 Stores attendance logs in `.csv` format
- 🗑️ User deletion with auto-model retraining
- 🧾 Web interface using Flask

---

## 🛠️ Tech Stack

| Purpose               | Technology          |
|----------------------|---------------------|
| Backend Web Framework| Flask               |
| Image Processing     | OpenCV              |
| Machine Learning     | scikit-learn (KNN)  |
| Data Handling        | Pandas, NumPy       |
| Serialization        | joblib              |
| UI Templates         | HTML (Jinja2)       |

---

## 📂 Project Structure

```
facial-attendance/
├── Attendance/                  # Stores attendance CSV files
├── static/
│   └── faces/                   # Contains folders for each user's face images
│   └── face_recognition_model.pkl # Saved KNN model
├── templates/
│   ├── home.html                # Homepage with attendance display
│   └── listusers.html           # Displays registered users
├── haarcascade_frontalface_default.xml
├── app.py                       # Main Flask app
├── README.md                    # This file
```

---

## 🔍 How It Works

### 1. **Face Registration**
- A new user provides a **name** and **roll number**.
- System captures `10` images using the webcam.
- Faces are detected using Haar Cascade (`haarcascade_frontalface_default.xml`).
- Resized and saved to `static/faces/<username_roll>/`.

### 2. **Training the Model**
- Images from all user folders are loaded and flattened.
- A **K-Nearest Neighbors (KNN)** model is trained on this data.
- Trained model is saved as `static/face_recognition_model.pkl`.

### 3. **Taking Attendance**
- Webcam is turned on.
- Faces detected → Resized → Flattened.
- Recognized using the trained KNN model.
- If matched and not already marked:
  - Attendance is stored in `Attendance/Attendance-<date>.csv`.

### 4. **User Management**
- **List Users**: View all registered users.
- **Delete User**: Removes user images and retrains the model.

---

## 🖥️ How to Run

### Step 1: Install Dependencies
```bash
pip install opencv-python flask scikit-learn numpy pandas joblib
```

### Step 2: Run the App
```bash
python app.py
```

### Step 3: Open in Browser
Visit [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## 🧪 Functional Overview

| Function            | Description                                                                 |
|---------------------|-----------------------------------------------------------------------------|
| `extract_faces()`   | Detects faces from webcam frame                                             |
| `train_model()`     | Trains the KNN model on registered users                                    |
| `identify_face()`   | Predicts face label using the saved model                                   |
| `add_attendance()`  | Writes name, roll, and time into daily CSV                                  |
| `deleteuser()`      | Deletes a user and retrains model                                           |
| `start()`           | Captures live webcam feed and marks attendance for recognized faces         |
| `add()`             | Adds new users with 10 face captures                                        |

---

## ✅ To-Do / Future Improvements

- Add **face recognition with deep learning** (e.g., FaceNet, Dlib)
- Improve **face detection accuracy** using MTCNN or YOLO
- Secure web interface with **authentication**
- Export attendance in **PDF** or **Excel** formats
- Deploy on **cloud** (e.g., Heroku, Render)

---

## 🙌 Acknowledgements

- [OpenCV](https://opencv.org/)
- [Flask](https://flask.palletsprojects.com/)
- [scikit-learn](https://scikit-learn.org/)
- [Haar Cascade Classifier](https://github.com/opencv/opencv/tree/master/data/haarcascades)

---

## 🧑‍💻 Author

**Parth Prasad Awasthi**  
_Artificial Intelligence and Machine Learning student at USAR, GGSIPU_  
President, **Intel oneAPI Students Club, EDC GGSIPU**  
[LinkedIn](https://www.linkedin.com/in/parthawasthi19/) • [GitHub](https://github.com/parthawasthi19)
