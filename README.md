# Shirts Detection Using YOLOv8n

## Project Overview
This project aims to detect and classify shirts of four colors—black, blue, white, and grey—using the YOLOv8 architecture. Data augmentation techniques are applied through Albumentations to improve model performance. The project involves data preparation, model training, and testing on images and real-time camera input.

## Dataset
The dataset comprises images of shirts in four classes:
- **Black shirt**: 150 images
- **Blue shirt**: 150 images
- **White shirt**: 150 images
- **Grey shirt**: 150 images

## Data Split
- **Training set**: 480 images (120 images per class)
- **Validation set**: 120 images (30 images per class)

## Data Augmentation
Data augmentation is performed using the Albumentations library, incorporating techniques such as:
- Random cropping
- Rotation
- Scaling
- Flipping
- Color adjustments

## Model Training
The YOLOv8n model is trained using both augmented and non-augmented datasets.

### Training Details:
- **Framework**: YOLOv8
- **Optimizer**: Adam
- **Loss Function**: YOLO loss
- **Batch Size**: 16
- **Epochs**: 100
- **Learning Rate**: 0.001

## Testing
The model is evaluated on a separate set of test images and real-time camera feed. Performance metrics include:
- **Recall (R)**: 91.9%
- **mAP@50**: 96.6%
- **mAP@50-95**: 90.3%

## Setup and Installation
1. Clone the repository:
   git clone https://github.com/majidhanif230/Shirt_Detection_Yolov8n.git
2. Navigate to the project directory:
   cd Shirt_Detection_Yolov8n
3. Create and activate a virtual environment:
  
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate'
  
4. Install the required packages:
   pip install ultralytics
   pip install albumentations

## Usage
- **Training the model**:
  - For augmented data: `Shirt_Model_Train(Argumentation).ipynb`
  - For non-augmented data: `Shirt_Model_Train.ipynb`
- **Testing the model**:
  - Run: `Yolo_Shirt_Testing.ipynb`

## Project Attribution
This project was provided by Machine Learning 1 Pvt Ltd and completed by Majid Hanif.
