# RoadSight — ML Mini-Project

## Project Overview
RoadSight is a road-hazard detection project. This experiment focuses on pothole detection using YOLO object-detection models.

## Dataset
- Images: 665 annotated images
- Classes evaluated: Pothole
- Training images: 426
- Validation images: 106
- Test images: 133
- Test instances: 299

## Models Compared
Four YOLO model variants were trained and evaluated using the same test split.

| Model | Precision | Recall | mAP@50 | mAP@50–95 |
|---|---:|---:|---:|---:|
| YOLOv8n | 78.66% | 70.57% | 80.19% | 49.99% |
| YOLOv8s | 78.41% | 69.57% | 78.41% | 49.18% |
| YOLO11n | 75.27% | 71.91% | 78.62% | 50.05% |
| YOLO11s | 80.14% | 68.56% | 79.93% | 51.25% |

## Conclusion
YOLOv8n achieved the highest mAP@50 in this experiment. YOLO11n achieved the highest recall, while YOLO11s achieved the highest precision and mAP@50–95. Model selection should also consider inference speed, model size, and deployment requirements.

## Limitations
- The current experiment detects potholes only.
- Speed-breaker detection requires suitable labeled data and additional training.
- Results apply to this dataset split and experimental setup.

## Tools Used
- Python
- Ultralytics YOLO
- PyTorch
- Google Colab
- Tesla T4 GPU

## Reproducibility
The notebook contains the training and evaluation workflow. Dataset availability, licensing, and model-weight availability should be checked before reuse.
