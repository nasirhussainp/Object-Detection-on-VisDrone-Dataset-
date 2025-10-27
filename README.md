# Object-Detection-on-VisDrone-Dataset-
Object Detection on VisDrone Dataset   
Project Overview  
This project applies object-detection techniques to the VisDrone dataset — aiming to detect and recognize various object categories (pedestrians, vehicles, bicycles, etc.) in drone-captured images. The main goal is to train and evaluate a deep learning model to accurately detect objects and localize them (bounding-boxes) in complex, aerial scenes.

Dataset  
Source: The VisDrone dataset: drone-captured images with annotations for object detection.  
Note: The dataset is not included in this repository due to size/licensing constraints. You will download it separately.  
Format: Images (drone perspective) + annotation files (typically bounding boxes per object).  
Important characteristics:  
  - Aerial viewpoint (top/down/slanted)  
  - Varying object sizes, occlusion, cluttered backgrounds  
  - Multiple object classes (e.g., people, cars, bicycles)  
- You should include instructions on how/where to download the dataset (link to VisDrone website or Kaggle dataset page) and where to place it (e.g., `/data/` folder) before running the notebook.

Notebook / Code  
visdrone_object_detection.ipynb` (or your notebook file) contains the full pipeline:  
  1. Data loading & preprocessing  
  2. Parsing annotation format (VisDrone’s format) and preparing data for training  
  3. Model architecture choice (e.g., YOLOv5, Faster R-CNN, SSD)  
  4. Training loop, loss monitoring, checkpointing  
  5. Evaluation: metrics such as mAP over object classes, precision, recall  
  6. Visualisations of detection results on sample frames  
Ensure the notebook includes a clear explanation of each step, hyperparameters, training settings (epochs, batch size, augmentation used).
