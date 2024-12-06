# Seat Belt Detection Project  

## Description  
This project focuses on detecting seat belt usage using advanced machine learning techniques, including YOLOv8 and RCNN. The project includes multiple components for training, evaluation, and testing.  

## Folder Structure  

### Code Folder Contents  
1. *train_yolov8t_SeatBelt.ipynb*  
   - Purpose: Script for training the YOLOv8 model on the seat belt dataset.  
   - Key Features:  
     - Model training configuration and initialization.  
     - Real-time performance monitoring.  
     - Saving model weights.  

2. *SeatBelt_YOLO_Pipeline.ipynb*  
   - Purpose: A pipeline for testing the YOLOv8 model on seat belt data.  
   - Key Features:  
     - Real-time video or image analysis.  
     - Visualization of predictions with bounding boxes.  
     - Integration with datasets for evaluation.  

3. *Test_mAP_All_Runs.ipynb*  
   - Purpose: Script to calculate the mean Average Precision (mAP) of trained models across multiple runs.  
   - Key Features:  
     - Model performance evaluation.  
     - Supports comparison across different training configurations.  

4. *rcnntrail2.ipynb*  
   - Purpose: Experimentation with Region-Based Convolutional Neural Networks (RCNN) for seat belt detection.  
   - Key Features:  
     - Model training and evaluation.  
     - Comparative study with YOLOv8.  

## Prerequisites  
- Python >= 3.8  
- Recommended libraries: See requirements.txt  

## Installation  
1. Clone the repository:  
   ```bash  
   git clone <(https://github.com/venkatdurga/Seatbelt-Detection-Using-DW-YOLOv8-Model)>  
   cd code
