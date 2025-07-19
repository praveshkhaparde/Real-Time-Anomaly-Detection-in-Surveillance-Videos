# Real-Time Anomaly Detection in Surveillance Videos

This project implements a complete pipeline to detect, track, and identify anomalous behavior (specifically, fast-moving pedestrians) in surveillance footage using computer vision techniques. The system leverages the YOLOv5 object detector and the DeepSORT tracking algorithm.

## Overview

The primary goal of this project is to automatically flag unusual events in surveillance video, such as a person running through a scene where most people are walking. This is achieved by processing the video through a multi-stage pipeline that identifies individuals, tracks their movement over time, and analyzes their speed to determine if it constitutes an anomaly.


![Untitled video - Made with Clipchamp](https://github.com/user-attachments/assets/9d60118f-b008-4bd0-8657-76f6dcb8fac7)

