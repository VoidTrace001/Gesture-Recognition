# 👁️🤚 Gesture Recognition & Eye Tracking System

> A real-time computer vision system that detects hand gestures, full body gestures, head movements, and tracks eye gaze — built with Python, MediaPipe, and OpenCV.

![Python](https://img.shields.io/badge/Python-3.12+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-4.x-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-Google-FF6F00?style=for-the-badge&logo=google&logoColor=white)
![License](https://img.shields.io/badge/License-GPL--3.0-blue?style=for-the-badge)

---

## 📌 Overview

This project is a modular real-time **Gesture Recognition and Eye Tracking system** using computer vision. It processes live webcam input to detect and classify human gestures and eye movements — with three independent modules covering hand gestures, full body pose, head orientation, and eye gaze tracking.

Built entirely in Python using Google's **MediaPipe** framework and **OpenCV** for video processing, with **dlib** for facial landmark detection in the eye tracker module.

---

## ✨ Modules

### 🤚 Hand & Head Gesture Recognition
Detects hand gestures and head orientation in real time using MediaPipe Hands and Face Mesh landmarks.

### 🧍 Full Body Gesture Recognition
Tracks full body pose using MediaPipe Pose — detects posture and body movement patterns.

### 👁️ Eye Tracker
Tracks eye gaze direction and blink detection using dlib's 68-point facial landmark model.

---

## 🏗️ Project Structure

```
Gesture-Recognition/
│
├── eye_tracker/              # Eye gaze tracking & blink detection
├── full_body_gesture/        # Full body pose detection
├── hand_head_gesture/        # Hand & head gesture recognition
│
├── shape_predictor           # dlib facial landmark model
├── requirements.txt          # Python dependencies
├── LICENSE
└── README.md
```

---

## 🚀 Setup & Installation

### 1. Clone the repository
```bash
git clone https://github.com/VoidTrace001/Gesture-Recognition.git
cd Gesture-Recognition
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Install dlib (Windows)
dlib requires a prebuilt wheel on Windows. Install it with:
```bash
pip install dlib-19.24.99-cp312-cp312-win_amd64.whl
```
> For Linux/Mac, dlib can be installed directly via `pip install dlib`

### 4. Run a module
```bash
# Eye Tracker
python eye_tracker/eye_tracker.py

# Full Body Gesture
python full_body_gesture/full_body.py

# Hand & Head Gesture
python hand_head_gesture/gesture.py
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| **Python 3.12+** | Core language |
| **OpenCV** | Video capture & frame processing |
| **MediaPipe** | Hand, pose & face landmark detection |
| **dlib** | 68-point facial landmark model |
| **NumPy** | Numerical computations |

---

## 🤖 How It Works

```
Webcam Input
     │
     ▼
Frame Preprocessing (OpenCV)
     │
     ▼
Landmark Detection (MediaPipe / dlib)
     │
     ├──→ Hand landmarks  →  Gesture classification
     ├──→ Pose landmarks  →  Body gesture detection
     ├──→ Face landmarks  →  Head orientation
     └──→ Eye landmarks   →  Gaze tracking & blink detection
     │
     ▼
Real-time Output (Annotated video feed)
```

---

## 📋 Requirements

See `requirements.txt` for the full list. Key dependencies:

- `opencv-python`
- `mediapipe`
- `dlib`
- `numpy`
- `imutils`

---

## 💡 Use Cases

- **Accessibility tools** — hands-free computer control
- **HCI research** — human-computer interaction studies
- **Security systems** — gaze-based authentication
- **Gaming** — gesture-controlled interfaces
- **Sign language detection** (extendable)

---

## 👤 Author

**VoidTrace001**  
🔗 [GitHub Profile](https://github.com/VoidTrace001)

---

*If you found this useful, consider leaving a ⭐!*
