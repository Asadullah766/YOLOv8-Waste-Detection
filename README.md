# YOLOv8-Waste-Detection
YOLOv8-based object detection project for identifying various waste materials in images. Includes training, validation, and inference workflows with preprocessed dataset for accurate predictions.


This project uses **YOLOv8 Nano** model for detecting 18 types of waste in images. The model is trained on a custom dataset with balanced classes and supports inference on new images.

## Features
- Detects 18 types of waste, including Aluminium foil, Bottle cap, Bottle, Broken glass, Can, Carton, Cigarette, Cup, Lid, Other litter, Paper, Plastic items, Pop tab, Straw, Styrofoam piece, and Unlabeled litter.
- Balanced dataset using augmentation to improve accuracy.
- Trained using **YOLOv8n** (Nano) for fast training with lower GPU requirements.

## Dataset
- Split into Train, Validation, and Test sets.
- YOLO format labels with images.

## Model Improvements
- **Current model:** YOLOv8 Nano (YOLOv8n) – lightweight and fast, suitable for limited GPU.
- **Suggestions for better accuracy:**
  - YOLOv8 Small (YOLOv8s) or Medium (YOLOv8m) – more parameters, better detection but slower.
  - Increase dataset size with more diverse images.
  - Apply advanced augmentations (mosaic, mixup, color jitter) during training.
  - Fine-tune learning rate and image size (`imgsz`) for your dataset.
  
## Installation
```bash
git clone https://github.com/Asadullah766/YOLOv8-Waste-Detection.git
pip install ultralytics opencv-python matplotlib
