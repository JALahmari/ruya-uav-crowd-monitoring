# Ru’ya — Lightweight UAV-Based Crowd Detection and Monitoring

Ru’ya is a graduation project exploring computer vision for crowd monitoring from an aerial/UAV perspective. This repository brings together the React dashboard and the YOLOv8 training and inference notebooks.

## Project goals
- Explore person detection in drone-view imagery using YOLOv8.
- Document the VisDrone training workflow and inference demo.
- Present crowd-monitoring information through a dashboard interface.
- Consider detection quality, inference speed, and deployment constraints.

## Repository structure
```text
.
├── src/                       # React dashboard application
├── public/                    # Public frontend assets
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
The dashboard is a React application built with Vite. It includes dashboard, analytics, alerts, flight-control, settings, and logs pages. The UI repository alone does not establish that a live UAV or model backend is connected.

### Run locally
Requirements: Node.js and npm.

```bash
npm install
npm run dev
```

To create a production build:
```bash
npm run build
npm run preview
```

## Model notebooks
- [VisDrone YOLOv8 training notebook](notebooks/01_Training_VisDrone_YOLOv8.ipynb)
- [Ru’ya inference demo notebook](notebooks/02_Final_Inference_Demo.ipynb)

The notebooks may require a GPU and separately downloaded datasets/model weights. Update input paths for your environment before running them. The inference notebook uses local model/video files that are not included in this repository.

## Datasets and reproducibility
The project report discusses public datasets including VisDrone, DroneCrowd, and WiderPerson. Dataset licenses and redistribution conditions vary; obtain data from the official sources and do not commit dataset files unless redistribution is explicitly allowed.

Report results only alongside the model variant, data split, metrics, hardware, and inference settings used. Do not describe planned UAV deployment or simulation as completed real-world flight testing.

## Team
Add the final approved team member names, roles, and supervisor acknowledgements before public release.

## Responsible use
This project is intended as a research prototype for crowd-safety support. Model outputs are estimates and should not be used as the sole basis for emergency decisions. Consider privacy, permissions, and applicable regulations before collecting or processing real crowd footage.

## License
No license has been selected in this repository. Confirm team ownership and university requirements before adding a license or claiming that others may reuse the code.
