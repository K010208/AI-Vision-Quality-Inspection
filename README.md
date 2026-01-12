AI-Vision-Quality-Inspection

Automated computer vision and vision–language solutions for industrial quality inspection, including object detection, PCB defect detection, and a hallucination-free Vision–Language Model (VLM) design for manufacturing environments.

Repository Overview

This repository contains solutions for a Computer Vision Engineer Assignment, focusing on real-world industrial inspection problems. The project demonstrates both traditional computer vision and deep learning-based approaches, along with a custom VLM system design suitable for offline deployment.

Project Structure
AI-Vision-Quality-Inspection/
│
├── Task1_Object_Detection/
│   ├── dataset/
│   ├── model/
│   ├── training/
│   └── results/
│
├── Task2_Quality_Inspection/
│   ├── images/
│   ├── annotations/
│   ├── results/
│   ├── step1_dataset_generation.py
│   └── step2_defect_detection.py
│
├── Task3_Custom_VLM/
│   ├── design_document.md
│   └── task3_custom_vlm.py
│
├── requirements.txt
└── README.md

Task 1: Custom Object Detection Model
Objective

Build and train an object detection model from scratch (without pre-trained weights) on a custom dataset.

Key Features

Custom CNN-based object detector

Training from scratch

Multiple object classes

Evaluation using:

Mean Average Precision (mAP)

Inference speed (FPS)

Model size

Visualization of detection results

Output

Trained model weights

Detection visualizations

Performance metrics

Task 2: Automated Quality Inspection System for Manufacturing
Objective

Develop an automated visual inspection system to detect defects in manufactured products (PCBs).

Defect Types

Scratches

Missing components

Misalignment

Step 1: Dataset Generation

Synthetic PCB image generation

Defective and non-defective samples

Bounding box annotations

JSON-based annotation format

Step 2: Defect Detection and Classification

Traditional computer vision-based defect detector

CNN-based defect detection model architecture

Defect localization using bounding boxes

Output includes:

Defect type

Confidence score

Severity assessment

(x, y) pixel coordinates of defect centers

Output

Annotated images

Detection result JSON files

Visual inspection dashboards

Task 3: Custom Vision–Language Model (VLM) Design for Industrial Inspection
Objective

Design an offline Vision–Language Model that answers natural language queries about PCB defects without hallucination.

Key Challenges Addressed

No QA pairs available

High hallucination risk in generic VLMs

Strict latency requirement (<2 seconds)

Offline deployment

Proposed Solution

Detector-first VLM architecture

Vision module grounded defect detection

Language module constrained to structured outputs

Hallucination mitigation through grounding and schema enforcement

Deliverables

Detailed system design document

Prototype implementation demonstrating:

Defect counting

Location-based queries

Severity summaries

Note: Task 3 is design-oriented. The provided code is a proof-of-concept demonstration.

Technologies Used

Python

OpenCV

NumPy

Matplotlib

PyTorch

scikit-learn

Setup Instructions

Clone the repository:

git clone https://github.com/<your-username>/AI-Vision-Quality-Inspection.git
cd AI-Vision-Quality-Inspection


Install dependencies:

pip install -r requirements.txt


Run Task 2 (example):

python Task2_Quality_Inspection/step1_dataset_generation.py
python Task2_Quality_Inspection/step2_defect_detection.py

Results

Accurate localization of PCB defects

Structured and interpretable defect reports

Hallucination-free VLM responses

Modular and scalable system design

Notes

All solutions are compatible with x86_64 and ARM architectures.

No pre-trained models were used unless explicitly stated.

Task 3 emphasizes architectural reasoning rather than full-scale training.

Author

Khushi Chauhan
