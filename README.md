# 👁️‍🗨️ Anti-Shoulder Surfing System

This project is a **privacy protection tool** that uses your laptop's webcam to detect **unauthorized persons appearing behind you** while you're working. It warns you in real-time if a second person enters the frame, helping prevent shoulder surfing attacks — especially useful in public spaces like cafes, co-working areas, and offices.

---

## 🚀 Features

- 👤 Captures or loads your face as the "trusted user"
- 🧠 Uses facial recognition to detect intruders
- 🚨 Alerts you visually when an unknown face is detected
- 🖥️ Real-time monitoring with your laptop camera
- 🔒 Adds an extra layer of privacy and awareness

---

## 🛠️ Tech Stack

- `Python`
- `OpenCV`
- `face_recognition` (dlib + HOG/CNN-based face detection)
- `NumPy`

---

## ⚙️ How It Works

1. **Face Enrollment**:
   - At first run, it captures your face and stores it.
   - On subsequent runs, it loads this saved face for comparison.

2. **Real-Time Monitoring**:
   - Continuously captures webcam frames.
   - Detects and encodes all visible faces.
   - Compares them with your saved face.
   - If more than one face is seen **or** an unrecognized face is detected, a **warning is triggered**.

