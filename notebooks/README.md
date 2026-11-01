# Model Notebooks

This folder contains the training and inference workflows for Ru’ya.

## 1. VisDrone YOLOv8 Training

File: `01_Training_VisDrone_YOLOv8.ipynb`

This notebook prepares VisDrone annotations in YOLO format, configures the dataset, trains a YOLOv8 model, evaluates performance, and exports the model.

## 2. Inference Demo

File: `02_Final_Inference_Demo.ipynb`

This notebook loads trained weights, runs detection on an input video, saves an annotated output video, generates frame-level statistics, and visualizes selected results.

## Requirements

- Python and Jupyter Notebook
- Ultralytics YOLOv8
- OpenCV
- The dataset, trained weights, and input videos required by the selected notebook

Download datasets from their original sources and place files in your own working environment. Update notebook paths to match your environment before execution. Dataset files, trained weights, and input videos are not included in this repository.
