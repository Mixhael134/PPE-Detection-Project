# PPE-Detection-Project
# Real-Time PPE Detection Using Computer Vision

## Student

Michael Rodriguez

## Project Tier

Tier 2

## Problem Statement

Many workplaces such as construction sites and warehouses require workers to wear personal protective equipment (PPE) like helmets. However, supervisors cannot constantly monitor every worker. This can lead to safety violations and increased risk of injuries.

## Solution Overview

This project will build a computer vision system that detects PPE equipment in images. Using an object detection model, the system will identify workers and determine whether they are wearing safety helmets.

The system workflow will be:
Camera Image → YOLOv8 Object Detection → Detect Person + Helmet → Output detection results.

## Technical Approach

Computer Vision Technique: Object Detection
Model: YOLOv8
Framework: PyTorch with Ultralytics YOLO

YOLOv8 is used because it is fast and accurate for object detection tasks and can run close to real-time.

## Dataset

Dataset Name: SH17 Dataset for PPE Detection
Source: Kaggle

The dataset contains images of workers with labeled bounding boxes for PPE equipment such as helmets.

## Success Metrics

Primary Metric: Mean Average Precision (mAP)

Target:
85–90% detection accuracy

Secondary Metrics:

* Detection speed
* Real-time inference capability

## Resources

Compute: Google Colab GPU
Tools: Python, PyTorch, Ultralytics YOLOv8
Estimated Cost: $0
