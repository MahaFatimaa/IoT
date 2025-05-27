# ATM Monitoring System Using IoT

## Table of Contents

- [Overview](#overview)
- [Project Methodology](#project-methodology)
- [Implementation Workflow](#implementation-workflow)
- [Technologies Used](#technologies-used)
- [Components](#components)

## Overview

This project presents an IoT-based security monitoring system specifically designed for ATMs. The system integrates real-time video surveillance with deep learning algorithms to detect suspicious behavior, such as the presence of weapons. By using smart devices and automation, the system aims to enhance ATM safety, reduce criminal activity, and ensure secure banking access for users.

## Project Methodology

The core methodology involves using deep learning techniques to detect weapons, specifically pistols, in ATM CCTV footage. The focus is on object recognition using Convolutional Neural Networks (CNNs) to analyze live video streams. The system is designed to:

- Identify pistols in video frames through image classification.
- Locate weapons precisely using object localization.
- Combine both tasks in real-time with object detection.

Two major approaches are used for detection:

1. **Sliding Window Classification Models**: The image is scanned using a window that moves systematically to identify the presence of a weapon.
2. **Region Proposal/Object Detection Models**: Advanced detection frameworks such as the YOLO series are used to identify objects and predict bounding boxes with high accuracy and speed.

## Implementation Workflow

1. Define the objective: binary classification of CCTV frames for weapon detection.
2. Collect and prepare a labeled dataset with images of pistols and non-threatening objects.
3. Preprocess images for optimal model performance.
4. Train a CNN-based model using backpropagation and supervised learning.
5. Validate and evaluate the model using appropriate metrics (accuracy, precision, recall).
6. Integrate the trained model with a live CCTV feed for real-time detection.
7. Deploy the system on an edge device (e.g., ESP32 with camera module).
8. Trigger alerts to authorities if a weapon is detected in the monitored footage.

## Technologies Used

- Python
- TensorFlow or PyTorch (for model training)
- OpenCV (for image and video processing)
- YOLOv5 or YOLOv8 (for real-time object detection)
- MQTT or HTTP (for IoT communication)
- Embedded C/C++ (for ESP32 programming)
- Google Colab or Jupyter Notebooks (for model development)

## Components

- CCTV Camera (for capturing real-time video footage)
- ESP32 Microcontroller (for processing and transmitting data)
- GPU-enabled system (for training deep learning models)
