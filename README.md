# Fabric-Defect-Detection-
# Fabric Defect Detection Using Deep Learning

## Overview

This research project focuses on automated fabric defect detection using YOLO object-detection models. The aim is to identify and localize defects in textile images and investigate how architectural modifications affect detection performance.

The experiments progress from a baseline model to attention-based and small-object detection improvements, followed by a comparison with YOLOv11n and a final experimental workflow.

## Experiments Undertaken

### 1. YOLOv12n — Baseline

The original YOLOv12n model was implemented to establish baseline performance for fabric defect detection. Its results serve as the reference for evaluating subsequent modifications.

### 2. YOLOv12n + ECA

Efficient Channel Attention (ECA) was incorporated to help the model focus on more informative feature channels. This experiment investigates the effect of channel attention on defect detection.

### 3. YOLOv12n + P2

A P2 detection head was introduced to use higher-resolution feature maps. The objective was to improve the detection of small fabric defects that may be difficult to localize using lower-resolution features.

### 4. YOLOv12n + ECA + P2

The ECA module and P2 detection head were combined into one architecture, referred to as **B3**. This experiment evaluates the combined effect of channel attention and higher-resolution detection features.

### 5. YOLOv11n

YOLOv11n was explored as an additional model for comparison with the YOLOv12n-based experiments. This provides another reference point for studying model performance on the fabric defect detection task.

### 6. Final Experiment

The final notebook brings together the research workflow for further evaluation and analysis. The objective is to review the experimental results and identify the strengths and limitations of the tested approaches.

## Dataset

The project uses the Chenab Textiles fabric defect dataset with seven defect categories:

- Baekra
- Color issues
- Contamination
- Cut
- Gray stitch
- Selvet
- Stain

## Technologies Used

- Python
- PyTorch
- Ultralytics YOLO
- Jupyter Notebook
- Computer Vision and Deep Learning

## Repository Structure

```text
Fabric-Defect-Detection-/
│
├── README.md
└── Notebook/
    ├── Fabric_Defect_Detection_YOLO12n.ipynb
    ├── Fabric_Defect_Detection_YOLOv12n_ECA.ipynb
    ├── Fabric_Defect_Detection_YOLOv12n_P2.ipynb
    ├── Fabric_Defect_Detection_ECA_P2_YOLOv12n.ipynb
    ├── Fabric_Defect_Detection_YOLOV11n.ipynb
    └── Fabric_Defect_Detection_final.ipynb
```

## Conclusion

The project follows an experimental approach to fabric defect detection, beginning with YOLOv12n and progressively investigating ECA, P2, and their combination. YOLOv11n is also explored for comparison. The experiments help assess the impact of architectural changes on detection performance and provide a foundation for further improvements in automated textile inspection.

