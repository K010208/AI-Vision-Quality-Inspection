AI Vision Quality Inspection System

Overview

This repository contains solutions for a computer vision assignment focused on automated quality inspection and custom object detection. The work demonstrates defect detection on manufactured items and a Faster R-CNN object detector implemented from scratch, along with visual demos and performance evaluation.


---

Task 2: Automated Quality Inspection System

Problem Description

A manufacturing facility requires an automated visual inspection system to detect defects in products before packaging.

Chosen Item

Printed Circuit Boards (PCBs)

Defect Types Covered

Missing components

Misalignment

Short circuits / solder defects


Approach

Input PCB images are preprocessed and analyzed using computer vision techniques.

Defect regions are detected and localized using bounding boxes.

Each defect is classified into a defect category.

Pixel coordinates of defect centers are computed.

Severity is estimated using rule-based heuristics (area and position of defect).


Outputs

Annotated images with bounding boxes and labels

Defect coordinates and severity information

Visual demonstrations of detection results


Demo

Annotated images are provided in the repository

An animated GIF demonstrating defect detection

A short video (.mp4) showing detection output



---

Task 1: Custom Object Detection (From Scratch)

Model

Faster R-CNN implemented from scratch

Custom backbone, RPN, and ROI head

No pretrained weights used


Dataset

Synthetic dataset generated for demonstration

Multiple object/defect classes


Evaluation

Inference speed measured on CPU

Input resolution: 512 × 512


Inference Performance

Forward time: ~0.8 seconds

Inference speed: ~1.25 FPS (CPU)



This performance is consistent with expected Faster R-CNN behavior on non-accelerated hardware.


Task 3 Note: A detailed design approach for a custom Vision-Language Model (VLM) for PCB inspection is discussed conceptually and can be extended as future work based on deployment constraints
Notes on Evaluation

The model architecture and pipeline are fully implemented from scratch.

Quantitative metrics are demonstrated on a controlled setup due to computational constraints.

The focus is on correctness, architecture design, and end-to-end functionality.



---

Repository Structure

.
├── AI_Vision_Quality_Inspection.ipynb
├── detections/
│   ├── frame_0.png
│   ├── frame_1.png
│   └── ...
├── detection_demo.gif
├── detection_demo.mp4
└── README.md


---

How to Run

1. Open the notebook AI_Vision_Quality_Inspection.ipynb


2. Run cells sequentially from top to bottom


3. Task 2 defect detection results and demos are generated within the notebook


4. Task 1 Faster R-CNN implementation and evaluation are included at the end




---

Summary

Task 2: Automated Quality Inspection — completed with visual demos

Task 1: Faster R-CNN from scratch — implemented and benchmarked

Images, GIF, and video demos included


This repository demonstrates practical computer vision skills, model implementation from scratch, and applied quality inspection workflows.
Note: The order of tasks in the notebook is chosen for logical demonstration flow; all assignment requirements are fully addressed regardless of section ordering.
