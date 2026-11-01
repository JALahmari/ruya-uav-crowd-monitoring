# Ru’ya: Lightweight UAV-Based Crowd Detection and Monitoring

Ru’ya is a graduation project exploring computer vision for crowd monitoring from an aerial perspective. The project combines a YOLOv8-based person-detection workflow with a web dashboard for presenting crowd-monitoring information.

## Project overview

The project focuses on:
- Detecting people in drone-view imagery using YOLOv8.
- Training and evaluating a model with the VisDrone dataset workflow.
- Running inference on video and collecting frame-level statistics.
- Presenting monitoring information through a React dashboard.

## Repository structure

```text
.
├── src/                         # React dashboard source
├── public/                      # Dashboard assets
├── notebooks/
│   ├── 01_Training_VisDrone_YOLOv8.ipynb
│   ├── 02_Final_Inference_Demo.ipynb
│   └── README.md
├── docs/
│   └── project-overview.md
├── dashboard/
│   └── README.md
├── package.json
└── README.md
```

## Dashboard

The dashboard is built with React and Vite. Its pages include Dashboard, Analytics, Alerts, Flight Control, Settings, and Logs.

### Run the dashboard locally

**Requirements:** Node.js and npm.

```bash
npm install
npm run dev
```

To build and preview the production bundle:

```bash
npm run build
npm run preview
```

## Model notebooks

1. **[VisDrone YOLOv8 training](notebooks/01_Training_VisDrone_YOLOv8.ipynb)** — prepares the VisDrone annotations for YOLO format, trains a YOLOv8 model, and evaluates the resulting weights.
2. **[Ru’ya inference demo](notebooks/02_Final_Inference_Demo.ipynb)** — runs inference on a video, overlays detections, calculates frame-level statistics, and saves output artifacts.

The notebooks require separately obtained datasets, model weights, and input videos. Update file paths to match your environment before running them. Large datasets, trained weights, and sample videos are not stored in this repository.

## Technology stack

- Python
- Ultralytics YOLOv8
- OpenCV
- Jupyter Notebook
- React
- Vite



