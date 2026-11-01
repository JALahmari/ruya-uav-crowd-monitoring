# Ru’ya — Lightweight UAV-Based Crowd Detection and Monitoring

Ru’ya is a graduation project exploring computer vision for crowd monitoring from an aerial perspective. It combines a YOLOv8-based person-detection workflow with a React dashboard for presenting crowd-monitoring information.

## Features

- Person-only object-detection training workflow using VisDrone annotations.
- YOLOv8 model evaluation and ONNX export.
- Video inference with annotated detections.
- Grid-based crowd-monitoring indicators and frame-level statistics.
- React dashboard with Dashboard, Analytics, Alerts, Flight Control, Settings, and Logs pages.

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

## Dashboard setup

**Requirements:** Node.js and npm.

```bash
npm install
npm run dev
```

Create and preview a production build:

```bash
npm run build
npm run preview
```

## Model notebooks

- [YOLOv8 training on VisDrone](notebooks/01_Training_VisDrone_YOLOv8.ipynb)
- [Ru’ya video inference demo](notebooks/02_Final_Inference_Demo.ipynb)

The training notebook expects the VisDrone dataset to be downloaded separately. Set DATASET_PATH in the notebook to the folder containing the VisDrone dataset directories. The inference notebook expects a trained best.pt model and an input video, such as drone_test.mp4, in its working directory. Update the paths in the configuration cell when needed.

Generated model weights, datasets, videos, and CSV outputs are excluded from version control.

## Technology stack

Python · Ultralytics YOLOv8 · OpenCV · Jupyter Notebook · React · Vite

## Project team

- **Esra Aldhayyan** — Project Leader
- **Dalya Alqahtani** — Planning Manager
- **Sajedah Alqudaihi** — Software Design
- **Joud Alahmari** — Software Development
- **Sarah Alashgar** — Testing

## Scope

Ru’ya is a computer-vision prototype for UAV-view crowd monitoring. The repository includes a web dashboard and separate model training/inference workflows; the repository does not establish a live connection between the dashboard and model or a deployed autonomous UAV system.
