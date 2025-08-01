# Real-Time Anomaly Detection in Surveillance Videos

This project implements a complete pipeline to detect, track, and identify anomalous behavior (specifically, fast-moving pedestrians) in surveillance footage using computer vision techniques. The system leverages the YOLOv5 object detector and the DeepSORT tracking algorithm.

## Overview

The primary goal of this project is to automatically flag unusual events in surveillance video, such as a person running through a scene where most people are walking. This is achieved by processing the video through a multi-stage pipeline that identifies individuals, tracks their movement over time, and analyzes their speed to determine if it constitutes an anomaly.


![Untitled video - Made with Clipchamp](https://github.com/user-attachments/assets/9d60118f-b008-4bd0-8657-76f6dcb8fac7)

## Project Structure

### 🔹 `image_processing/`
Contains basic image processing utilities using the OpenCV (`cv2`) Python library. Includes:
- Image transformations (grayscale, blur, edge detection)
- Webcam integration
- Utility scripts for visualization

### 🔹 `object_detection/`
Implements object detection pipelines using YOLOv5. Covers:
- Pretrained YOLOv5 models (`v5s`, `v5m`, etc.)
- Custom dataset training and inference
- Evaluation and visualization scripts

### 🔹 `deep_sort/`
Core implementation of the DeepSORT tracking algorithm integrated with YOLOv5 for real-time multi-object tracking.

### 🔹 `MOT_detection+tracking/` & `assignment/`
Detection and tracking workflows applied to the **MOT17 dataset**. Includes:
- Integration scripts
- Tracking visualizations
- Metric evaluation

### 🔹 `Avenue/`
Anomaly detection module applied to the **Avenue dataset**. The system identifies abnormal motion patterns—particularly **fast-moving pedestrians**—using bounding box displacement and temporal analysis over tracked trajectories.

---

## Key Features

- ✅ Real-time object detection using YOLOv5
- ✅ Multi-object tracking via DeepSORT
- ✅ Speed-based anomaly detection in pedestrian motion
- ✅ Modular folder structure for scalability and reproducibility
- ✅ Visualization-ready outputs and video overlays

---

## Anomaly Definition

In this project, an **anomaly** is defined as a pedestrian moving significantly faster than the average crowd movement—typically a person **running** in an environment where walking is the norm. These are automatically flagged based on motion statistics derived from tracking data.

---

## Dependencies

- Python 3.8+
- OpenCV
- PyTorch
- YOLOv5 (from Ultralytics)
- NumPy, Matplotlib
- torchvision, scipy

---

## Example Use Cases

- Intelligent surveillance systems
- Crowd behavior analytics
- Security monitoring for public transport hubs, malls, etc.
