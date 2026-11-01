# Ru’ya Project Overview

## Motivation

Crowded public events create challenges for timely observation and situational awareness. Ru’ya explores the use of computer vision on aerial imagery as a potential aid for crowd monitoring.

## Approach

The project uses a YOLOv8-based person-detection workflow. The training notebook prepares VisDrone annotations for YOLO format and runs model training and evaluation. The inference notebook processes video, overlays detections, and records frame-level statistics. A React dashboard provides an interface for presenting monitoring information.

## Main components

- **Model training:** `notebooks/01_Training_VisDrone_YOLOv8.ipynb`
- **Inference demo:** `notebooks/02_Final_Inference_Demo.ipynb`
- **Dashboard:** React and Vite application in the repository's `src/` directory

## Technologies

Python, Ultralytics YOLOv8, OpenCV, Jupyter Notebook, React, and Vite.

## Team

- Esra Aldhayyan — Project Leader
- Dalya Alqahtani — Planning Manager
- Sajedah Alqudaihi — Software Design
- Joud Alahmari — Software Development
- Sarah Alashgar — Testing
