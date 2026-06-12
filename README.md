# 🚁 Drone Detection using YOLO11

## 📌 Overview

This project implements a real-time drone detection system using **YOLO11**, a state-of-the-art object detection framework designed for high-speed and accurate object localization.

The model is trained to detect drones in images, video streams, and live camera feeds. By leveraging YOLO11's efficient architecture, the system can accurately identify drones across various environments, scales, and lighting conditions while maintaining real-time performance.

---

## 🎯 Objective

The primary goal of this project is to build a robust computer vision model capable of detecting drones under challenging real-world conditions, including:

* Small and distant drones
* Complex backgrounds
* Different weather and lighting conditions
* Multiple viewing angles
* Dynamic scenes

---

## 📂 Dataset

The model was trained on a custom drone detection dataset annotated in YOLO format.

### Dataset Features

* Single-class object detection
* Drone bounding box annotations
* Diverse environments and backgrounds
* Various drone sizes and orientations
* Background-only images included to reduce false detections

### Class Labels

| ID | Class |
| -- | ----- |
| 0  | Drone |

---

## 🧠 Model

This project uses **YOLO11** for object detection.

YOLO11 performs:

* Feature extraction
* Object localization
* Confidence estimation

in a single forward pass, enabling efficient real-time inference.

### Detection Output

For every detected drone, the model predicts:

* Bounding box coordinates
* Confidence score
* Class label

---

## 🏋️ Training

The model was trained using the Ultralytics YOLO11 framework.

### Training Pipeline

1. Dataset preparation
2. Data augmentation
3. Model training
4. Validation monitoring
5. Best-weight selection

### Data Augmentation

To improve generalization, training includes:

* Horizontal flipping
* Scaling
* Translation
* Rotation
* Mosaic augmentation
* Color-space transformations

---

## ⚡ Real-Time Inference

The trained detector supports:

* 📷 Images
* 🎥 Video files
* 📹 Webcam streams
* 🛰️ Surveillance camera feeds

### Detection Workflow

1. Load trained YOLO11 weights
2. Read input frame
3. Perform drone detection
4. Predict bounding boxes
5. Draw detections
6. Display confidence scores
7. Output final results

---

## 📊 Results

The model successfully detects drones across a wide range of environments while maintaining efficient inference speed.

Performance improvements were achieved through:

* YOLO11 architecture
* Diverse training data
* Background-only images
* Data augmentation techniques

---

## 🛠️ Technologies Used

* Python
* PyTorch
* Ultralytics YOLO11
* OpenCV
* NumPy

---

## 🚀 Applications

* Airspace Monitoring
* Drone Surveillance
* Security Systems
* Smart Cities
* Autonomous Monitoring
* Restricted Area Protection
* UAV Detection and Tracking
