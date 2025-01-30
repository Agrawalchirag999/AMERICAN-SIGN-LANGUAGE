# American Sign Language (ASL) Detection Project

## Overview
This project focuses on real-time American Sign Language (ASL) detection using computer vision and deep learning techniques. It utilizes MediaPipe for hand landmark detection and a trained neural network model to classify ASL signs.

## Project Structure
The project consists of three main components:
1. **Dataset Generator** - Captures hand landmarks and stores them for model training.
2. **MediaPipe Hand Tracking** - Processes video frames to extract hand landmarks.
3. **Streamlit Application** - Provides an interactive interface for real-time ASL detection.

---

## 1️⃣ Dataset Generator
### Description
This module captures hand landmark coordinates from webcam input and stores them as a dataset for training the classification model.

### Features
- Uses **MediaPipe Hands** for hand landmark detection.
- Extracts and normalizes 21 hand keypoints.
- Saves data in a structured format for model training.

### Usage
Run the script to capture hand landmarks:
```bash
python dataset_generator.py
```

### Output
- CSV file containing landmark coordinates labeled with corresponding ASL signs.

---

## 2️⃣ MediaPipe Hand Tracking
### Description
This module processes real-time video input to detect and track hand landmarks using MediaPipe.

### Features
- Detects hands in real-time using **MediaPipe Hands**.
- Converts landmarks to a normalized format.
- Displays detected hand landmarks using OpenCV.

### Usage
Run the script to start hand tracking:
```bash
python media_pipe.py
```

### Output
- Displays real-time video feed with hand landmarks annotated.

---

## 3️⃣ ASL Detection with Streamlit
### Description
This module provides a user-friendly interface using Streamlit to predict ASL signs in real time.

### Features
- Loads a trained **Keras model** for ASL classification.
- Processes video frames and extracts hand landmarks.
- Predicts ASL signs using the trained model.
- Displays predictions in an interactive UI.

### Usage
Run the Streamlit app:
```bash
streamlit run app_streamlit.py
```

### Output
- A web-based interface displaying real-time ASL detection results.

---

## 🔧 Setup & Installation
### Requirements
- Python 3.8+
- OpenCV
- MediaPipe
- TensorFlow/Keras
- Pandas
- NumPy
- Streamlit

### Installation
Install dependencies using:
```bash
pip install -r requirements.txt
```

---

## 🚀 Future Enhancements
- Improve model accuracy with more training data.
- Support for dynamic ASL gestures.
- Deploy as a cloud-based web application.

---


