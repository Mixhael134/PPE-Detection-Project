# PPE-Detection-Project

# Real-Time PPE Detection Using Computer Vision

## Student

Michael Rodriguez

## Project Tier

Tier 2

---

# Problem Statement

Many workplaces such as construction sites and warehouses require workers to wear personal protective equipment (PPE) like helmets and safety vests. Supervisors cannot constantly monitor every worker, which can lead to safety violations and increased risk of injuries.

This project explores how computer vision can automatically detect PPE equipment in workplace environments.

---

# Solution Overview

This project uses a YOLOv8 object detection model to detect workers and PPE equipment in images.

The system workflow is:

Camera Image → YOLOv8 Object Detection → Detect Person, Helmet, and Vest → Display Detection Results

The trained model generates bounding boxes around detected PPE equipment and workers in validation images.

---

# Technical Approach

## Computer Vision Technique

Object Detection

## Model

YOLOv8n

## Framework

Python, PyTorch, Ultralytics YOLOv8

YOLOv8 was selected because it provides fast and accurate real-time object detection performance while remaining lightweight enough to train in Google Colab.

---

# Dataset

## Dataset Name

SH17 Dataset for PPE Detection

## Source

[Kaggle](https://www.kaggle.com/datasets/mugheesahmad/sh17-dataset-for-ppe-detection)

## Classes

* person
* helmet
* vest

The dataset contains labeled images of workers wearing personal protective equipment.

---

# Results

The model was successfully trained using YOLOv8 and generated detection predictions on validation images.

## Evaluation Metrics

* Precision: ~1.00 peak precision
* Recall: ~0.45 peak recall
* mAP50: ~0.13
* mAP50-95: ~0.10

## Outputs Generated

* Confusion Matrix
* Training Curves
* Validation Prediction Images
* Bounding Box Detections

Example outputs are included in the `results/` folder.

---

# Repository Structure

```text
PPE-Detection-Project/

├── data/
├── docs/
├── notebooks/
├── results/
├── README.md
└── requirements.txt
```

---

# Resources Used

## Compute

Google Colab GPU

## Tools

* Python
* PyTorch
* Ultralytics YOLOv8

## Estimated Cost

$0

---

# Challenges

Some challenges encountered during the project included:

* Small dataset size
* Dataset formatting for YOLOv8
* Lower recall performance on some PPE classes

These issues were addressed using dataset restructuring and YOLOv8 training adjustments.

---

# Future Improvements

Potential improvements for this project include:

* Training for more epochs
* Using larger YOLOv8 models
* Expanding the dataset
* Improving detection accuracy for helmets and vests
* Adding real-time webcam support

---

# Conclusion

This project successfully demonstrated how computer vision and YOLOv8 can be used for PPE detection in workplace environments. The system was able to generate object detections, evaluation metrics, and visual outputs using a real-world PPE dataset.
