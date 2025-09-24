# 🏳️ YOLOv8 Country Flags Detector

This project uses YOLOv8 to detect different country flags in images. The dataset was created by manually collecting flag images and combining them with additional data from Kaggle. Labeling was done with Roboflow, and the model was trained using the Ultralytics YOLOv8 framework.

## 🚀 Features

Detects multiple country flags in an image.

Trained with a custom dataset of manually collected + Kaggle-sourced images.

Simple inference pipeline for running detection on any image.

## 📦 Installation

Clone the repository and install the required dependencies:

git clone https://github.com/yourusername/flag-detector.git
cd flag-detector
pip install ultralytics opencv-python

## 🏋️ Training

If you want to retrain the model on your own dataset:

```bash
yolo detect train data=flags.yaml model=yolov8n.pt epochs=50 imgsz=640
```

## 🔍 Inference

Run detection on an image:

yolo detect predict model=best.pt source="path/to/image.jpg"


The output with bounding boxes will be saved inside the runs/detect/predict folder.

## 📖 Acknowledgements

YOLOv8 by Ultralytics

Roboflow for labeling tools

Dataset partially from Kaggle + manually collected images
