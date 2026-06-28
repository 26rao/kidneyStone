# Automated Kidney Stone Detection and Severity Grading using Deep Learning on Radiographs

A two-stage deep learning pipeline for **automated detection, localization, and severity grading** of kidney stones from radiographic images (CT / Ultrasound). Designed to assist radiologists and urologists in faster and more consistent diagnosis.

---

## Overview

Kidney stones (nephrolithiasis) are a common and painful condition affecting millions worldwide. Manual detection and severity assessment on radiographs can be time-consuming and subject to inter-observer variability.  

This project proposes a **two-stage deep learning system** that:
1. **Localizes** kidney stones with high accuracy using object detection.
2. **Grades severity** (size, number, location, obstruction risk) using a regression/classification approach.

The system aims to reduce diagnostic time and improve clinical decision-making in urology and radiology departments.

---

## Methodology

### Two-Stage Pipeline

**Stage 1: Localization (Object Detection)**
- Uses **YOLOv8** (Ultralytics) to detect and localize kidney stones in radiographs.
- Outputs bounding boxes with confidence scores.

**Stage 2: Severity Grading**
- Crops the detected regions and feeds them into a **ResNet-18** based model.
- Performs regression for stone size and multi-class classification for severity levels.

### Key Features
- Robust preprocessing pipeline (normalization, resizing, augmentation)
- State-of-the-art object detection with YOLOv8
- Transfer learning on ResNet-18 for severity estimation
- End-to-end inference pipeline for clinical usability

---

## Dataset

- Publicly available kidney stone radiographic datasets (CT and Ultrasound)
- Images include varied stone sizes, locations, and imaging conditions
- Preprocessing steps: intensity normalization, contrast enhancement, geometric augmentations

---

## Technologies & Dependencies

- **Language**: Python 3.x
- **Deep Learning**: PyTorch, Ultralytics YOLOv8
- **Computer Vision**: OpenCV
- **Scientific Computing**: NumPy, Matplotlib, Pandas
- **Others**: Albumentations (for augmentation), scikit-learn

---

## Project Status

**Current Status**: Published \
**Publication**: https://www.sciencedirect.com/science/article/pii/S2352914825000930

---

## License

This project is for research purposes only. 

---

**Contact / Citation**
If you use this work in your research, please cite:
