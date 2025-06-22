# Real-Time Anomaly Detection in Surveillance Videos

A computer vision project implementing real-time video analysis for security applications, featuring OpenCV-based image processing and YOLOv5 object detection.

## Project Structure

### 📂 Image Processing
- **OpenCV-based real-time camera effects**
  - Live black & white conversion
  - Frame-by-frame processing pipeline
  - Webcam integration (`webcam_basic.ipynb`)

### 📂 Object Detection
- **YOLOv5-based vehicle detection** (small & medium models)
  - Detected classes: 🚗 Cars, 🚑 Ambulances, 🚛 Trucks, 🏍 Motorcycles
  - Implemented models:
    - `YOLOv5s` (faster, lower accuracy)
    - `YOLOv5m` (slower, higher accuracy)
  - Sample predictions available in `/predicted` folder

## Technical Stack
- Python 3.8+
- OpenCV 4.5+
- PyTorch 1.7+
- Ultralytics YOLOv5
- Jupyter Notebooks

## Setup Instructions
```bash
git clone https://github.com/praveshkhaparde/Real-Time-Anomaly-Detection-in-Surveillance-Videos.git
cd Real-Time-Anomaly-Detection-in-Surveillance-Videos
pip install -r requirements.txt
