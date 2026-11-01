# Ru’ya — Lightweight UAV-Based Crowd Detection and Monitoring

Ru’ya is a graduation project exploring how lightweight computer-vision models can support crowd monitoring from an aerial/UAV perspective. The project investigates object detection, crowd-related analysis, and a dashboard-oriented way to present results.

> **Project status:** This repository documents the project and links its main components. The training and inference notebooks are maintained separately until their contents are added here. Features, metrics, and deployment claims should be updated only from verified experiments.

## Project goals

- Explore UAV-view crowd detection using YOLOv8.
- Prepare and evaluate a detection workflow using public datasets.
- Compare lightweight model variants with attention to detection quality and inference speed.
- Present model outputs through a dashboard for easier inspection.

## Repository structure

```text
.
├── README.md
├── docs/
│   └── project-overview.md
├── notebooks/
│   └── README.md
└── dashboard/
    └── README.md
```

The dashboard source currently lives in this repository's existing application files. The `dashboard/` folder documentation explains its role; it does not replace the application source.

## Notebooks

The project workflow includes these notebooks:

- `01_Training_VisDrone_YOLOv8.ipynb` — model training workflow for VisDrone.
- `02_Final_Inference_Demo.ipynb` — final inference/demo workflow.

Add the notebooks to `notebooks/` after reviewing them for local paths, secrets, personal data, and dataset restrictions.

## Datasets

The project report discusses DroneCrowd, VisDrone, and WiderPerson. Dataset access, licenses, and redistribution rules differ; **do not upload dataset images or annotations unless their terms explicitly permit redistribution**. Link to official dataset sources and document the exact subset used.

## Getting started

1. Review the notebook and dashboard-specific instructions.
2. Install dependencies in a clean environment using the requirements documented for each component.
3. Obtain the datasets separately from their approved sources.
4. Update dataset paths in the notebooks for your environment.
5. Run training or inference only after verifying the dataset paths and model weights.

## Results and reproducibility

Add only measured results from the final experiments, including the model variant, dataset split, evaluation metrics, hardware, and inference settings. Do not treat planned UAV deployment or simulation as completed real-world flight testing.

## Team and contributions

Ru’ya was developed as a graduation project by a student team. Update this section with the agreed team member names, individual contributions, and supervisor acknowledgements before publishing.

## Responsible use

This project is intended for research and crowd-safety support. A model's detections are estimates and should not be treated as a sole basis for emergency decisions. Review privacy, permissions, and local regulations before collecting or processing real crowd footage.

## License

No license has been selected yet. Until a license is added, do not assume others have permission to reuse the code. Confirm team ownership and university requirements before choosing one.
