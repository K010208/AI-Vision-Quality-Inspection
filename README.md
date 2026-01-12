# Computer Vision Engineer Assignment

This repository contains the complete and final submission for the Computer Vision Engineer Assignment. All tasks have been implemented and documented as per the assignment requirements.

---

## Task 1: Custom Object Detection from Scratch

A custom object detection pipeline was implemented and trained from scratch without using any pre-trained weights.

### Implementation Details
- Custom CNN-based detection model
- Training and validation pipeline
- IoU-based mAP@0.5 evaluation
- Inference speed (FPS) benchmarking
- Model size estimation
- Real-time detection visualization

### Evaluation
- mAP@0.5: Computed using IoU-based matching
- Inference Speed: Measured in frames per second (FPS) on CPU
- Model Size: Calculated in megabytes (MB)
- Real-time Detection: Demonstrated using bounding box visualization and screen recording

This task demonstrates the balance between accuracy, inference speed, and model size in a custom detection pipeline.

---

## Task 2: Automated Quality Inspection System for Manufacturing

An automated visual inspection system was developed for PCB defect detection using a synthetic dataset.

### System Features
- Synthetic PCB dataset generation
- Defect-free and defective PCB samples
- Detection and localization of defects using bounding boxes
- Classification of multiple defect types
- Severity estimation for detected defects
- Annotation generation and visualization

### Defect Types
- Missing components
- Misalignment
- Surface defects

This system demonstrates an end-to-end quality inspection workflow suitable for manufacturing environments.

---

## Task 3: Custom Vision–Language Model (VLM) Design for PCB Inspection

A complete design document is provided for a custom Vision–Language Model tailored for industrial PCB inspection.

### Design Coverage
- Model selection and justification
- Vision and language architecture design
- Vision–language fusion strategy
- Optimization for offline inference (< 2 seconds)
- Hallucination mitigation strategies
- Multi-stage training plan
- Validation metrics and evaluation strategy

The design focuses on reliability, low latency, and accurate defect localization for industrial deployment.

---

## Repository Structure

AI-Vision-Assignment/ │ ├── notebooks/ │   └── AI_Vision_Quality_Inspection.ipynb │ ├── data/ │   ├── images/ │   └── annotations/ │ ├── results/ │   ├── task1_realtime_detection.mp4 │   └── sample_outputs/ │ ├── docs/ │   └── Task3_VLM_Design.md │ ├── requirements.txt └── README.md

---

## Environment and Dependencies

- Python
- PyTorch
- OpenCV
- NumPy
- Matplotlib

All code is compatible with Jupyter Notebook and Google Colab environments.

---

## Submission Notes

- All tasks have been implemented as per the assignment requirements
- The notebook runs without errors
- Quantitative outputs for mAP, FPS, and model size are included
- Real-time detection visualization is provided as image/video output
- The VLM design is documented separately

---

## Author

Khushi Chauhan
