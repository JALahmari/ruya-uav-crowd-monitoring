# Ru’ya Project Overview

Ru’ya explores computer vision as a potential aid for monitoring crowds from aerial imagery.

## Approach

The project uses a YOLOv8-based person-detection workflow. The training notebook converts VisDrone annotations to YOLO format, trains a model, evaluates its performance, and exports the model. The inference notebook processes video, overlays detections and grid-based monitoring indicators, and records frame-level statistics. A React dashboard presents the project's monitoring interface.

## Components

- **Model training:** [VisDrone YOLOv8 training notebook](../notebooks/01_Training_VisDrone_YOLOv8.ipynb)
- **Video inference:** [Inference demo notebook](../notebooks/02_Final_Inference_Demo.ipynb)
- **Dashboard:** React and Vite application in the repository's src/ directory

## Technologies

Python, Ultralytics YOLOv8, OpenCV, Jupyter Notebook, React, and Vite.

## Team

- Esra Aldhayyan — Project Leader
- Dalya Alqahtani — Planning Manager
- Sajedah Alqudaihi — Software Design
- Joud Alahmari — Software Development
- Sarah Alashgar — Testing
