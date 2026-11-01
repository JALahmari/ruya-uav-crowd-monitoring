# Project overview

## Motivation
Crowded public events can benefit from timely visual information. Ru’ya explores UAV-view computer vision as a potential aid for crowd monitoring.

## Approach
The project investigates a YOLOv8-based detection workflow, using public crowd/drone-view datasets discussed in the project report. Model evaluation and the inference demo are represented by the training and inference notebooks. A dashboard provides a visual interface for presenting project outputs.

## Components
- **Training notebook:** `01_Training_VisDrone_YOLOv8.ipynb`
- **Inference notebook:** `02_Final_Inference_Demo.ipynb`
- **Dashboard:** existing application source in the repository

## Before release
- Verify dataset citations, licenses, and exact splits.
- Add final metrics directly from experiment outputs.
- Document the dashboard setup and connect it to inference only if that integration is implemented.
- Remove private paths, tokens, credentials, and restricted data.
- Confirm the team and university permit public release.
