# Model Notebooks

This folder contains the model training and video inference workflows for Ru’ya.

## Training: VisDrone YOLOv8

File: 01_Training_VisDrone_YOLOv8.ipynb

The notebook prepares VisDrone annotations for person-only detection, trains a YOLOv8 model, evaluates metrics, and exports the model to ONNX.

Set DATASET_PATH to the location of the downloaded VisDrone dataset before running the notebook. Training may require a compatible GPU.

## Inference demo

File: 02_Final_Inference_Demo.ipynb

The notebook loads trained weights, processes a video, overlays detections and grid-based indicators, writes an annotated video, exports frame-level statistics, and saves selected frames for qualitative review.

Place best.pt and the input video in the notebook's working directory, or update their paths in the configuration cell. ONNX checking is optional.

## Outputs

The notebooks can generate model weights, annotated videos, CSV statistics, and failure-case images. These generated artifacts are excluded from version control.
