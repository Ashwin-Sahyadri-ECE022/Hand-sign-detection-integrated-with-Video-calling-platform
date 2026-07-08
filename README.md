<div align="center">
  <h1>🚀 Hand-sign-detection-integrated-with-Video-calling-platform</h1>
</div>

In this repository we will be going through how to setup a hand sign detection model from the training stage to the running stage, and then how to run it in a video calling platform
Below is a complete, clean `README.md` you can directly use for GitHub.

---

# Hand Sign Detection with Real-Time Video Calling (ISL)

## Overview

This project is a real-time **Hand Sign Detection and Communication System** based on **Indian Sign Language (ISL)** integrated with a **live video calling platform using Agora AI**.
It enables users to communicate through hand signs during a video call by detecting gestures and converting them into readable text in real time.

The system is designed to assist **deaf and mute individuals** by improving accessibility in video communication.

---

## Features

* Real-time hand sign detection using computer vision
* Supports Indian Sign Language (ISL) gestures
* Live video calling using **Agora AI SDK**
* Gesture-to-text conversion during video call
* Low latency real-time processing
* Works with standard webcam
* Scalable for future speech / audio integration

---

## System Architecture

```
Webcam → Hand Detection Model → Gesture Classification → Text Output
                                  ↓
                          Agora Video Call Stream
```

---

## Technologies Used

### Software

* Python
* OpenCV
* MediaPipe / Hand Tracking
* TensorFlow / Keras (for gesture model)
* Agora AI Video Calling SDK
* NumPy

### Hardware

* Laptop / PC with webcam
* Internet connection

---

## How It Works

1. Webcam captures live video.
2. Hand landmarks are detected using MediaPipe / vision model.
3. Gesture is classified using trained model.
4. Corresponding text is generated.
5. During **Agora video call**, detected text is displayed in real time.
6. The other user can read the translated sign instantly.

---

## Installation

### 1. Install Dependencies

```bash
pip install -r requirements.txt
```

### 2. Setup Agora

* Create account at [https://www.agora.io](https://www.agora.io)

* Create a new project

* Copy:

  * **App ID**
  * **Temporary Token** (or implement token server)

* Replace in config file:

```python
APP_ID = "your_app_id"
TOKEN = "your_token"
CHANNEL_NAME = "test"
```

---

## Running the Project

### Start Hand Sign Detection

```bash
python detect.py
```

### Start Video Call

```bash
python agora_call.py
```

Both modules run together for real-time gesture communication.

---

## Dataset

* Custom dataset based on **Indian Sign Language (ISL)**
* Includes multiple gesture samples per sign
* Preprocessed using hand landmark normalization

---

## Model

* Gesture Classification Model
* Input: Hand landmarks / processed image
* Output: ISL sign label
* Accuracy: (add your accuracy here)

---

## Use Case

* Communication aid for deaf and mute individuals
* Accessible video conferencing
* Assistive technology research
* Real-time gesture recognition systems

---

## Future Improvements

* Speech output (Text-to-Speech)
* Full sentence formation
* More ISL gesture coverage
* Mobile app integration
* Edge device deployment (ESP32 / Jetson / Raspberry Pi)
* Emotion / facial expression detection

---

## Project Structure

```
├── detect.py
├── agora_call.py
├── model/
├── dataset/
├── utils/
├── requirements.txt
└── README.md
```

---

## Author

**Ashwin Suresh**
Electronics and Communication Engineering

---

## License

This project is for academic and research purposes.



Request the version needed.


---

<div align="center">
  <h2><strong>👨‍💻 Connect with Me</strong></h2>
  <a href="https://github.com/Ashwin-Sahyadri-ECE022"><img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/ashwin-suresh-aa2573268"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:ashwinsuresh1122@gmail.com"><img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</div>
