# Face Recognition Attendance System

## Project Overview

This project is an **AI-based Face Recognition Attendance System** that automatically detects and recognizes faces using a webcam and marks attendance in a CSV file.

## **It uses:**

* OpenCV for face detection
* CNN / Transfer Learning (**MobileNetV2**) for face recognition
* TensorFlow/Keras for model training

---

## Features

* Real-time face detection using webcam
* Deep Learning-based face recognition
* Automatic attendance marking
* CSV file storage for attendance logs
* Duplicate entry prevention

---

## Tech Stack

* **Python**
* **OpenCV**
* **TensorFlow / Keras**
* **NumPy & Pandas**
* **Scikit-learn**

---

## 📂 Project Structure

```
Face-Recognition-Attendance/
│
├── Dataset/
│   ├── Person1/
│   ├── Person2/
│
├── attendance.csv
├── face_recognition_model.h5
├── haarcascade_frontalface_default.xml
├── Attendance_face-recognition.py
└── README.md
```

---

## ⚙️ Installation

### **1️⃣ Clone the Repository**

```sh
git clone https://github.com/your-username/face-attendance.git
cd face-attendance
```

### **2️⃣ Install Dependencies**

```sh
pip install opencv-python tensorflow numpy pandas scikit-learn
```

---

## Dataset Preparation

* Create a folder named **Dataset**
* Inside it, create subfolders for each person

**Example:**

```
Dataset/
├── Anushka/
├── Rahul/
```

* Add multiple face images for each person

---

## Model Training

### **CNN Model**

* Grayscale images (100x100)
* Simple architecture with Conv2D + Dense layers

### **MobileNetV2 (Transfer Learning)**

* RGB images (224x224)
* Better accuracy with data augmentation

---

## How to Run

```sh
python Attendance_face-recognition.py
```

---

## How It Works

* Detect face using Haar Cascade
* Preprocess face image
* Predict using trained model
* Display name on screen
* Mark attendance in CSV file

---

## Attendance Format

```
Name, Time
Anushka, 2026-05-05 10:30:21
Rahul, 2026-05-05 10:32:10
```

---

## Key Functions

### **preprocess_image()**

* Converts image to grayscale
* Resizes and normalizes

### **recognize_face()**

* Predicts the person using trained model

### **mark_attendance()**

* Stores name + timestamp in CSV
* Prevents duplicate entries

---

## 📈 Future Improvements

* Add Streamlit Web UI
* Multi-face tracking optimization
* Cloud database integration (AWS / Firebase)
  Mobile app integration

---

##  Notes

* Ensure correct path for:

  * Haar Cascade file
  * Dataset directory
* Webcam access is required

---

##  Author

**Anushka Gunjal**



