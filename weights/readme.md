# Weights Folder - Seat Belt Detection Project

This folder contains the trained model weights for different configurations of the Seat Belt Detection project. These weights are the result of training the YOLOv8 model with various architectures and datasets. Below is an overview of the files contained in this folder:

## Folder Structure and Files

1. *seatbeltWbest (1).pt*
   - *Description*: This is the model weight file for the YOLOv8 model that has been trained specifically on the seat belt detection dataset. It represents the best-performing model for detecting seat belt usage.
   - *Usage*: 
     - To continue training or fine-tune the model, load this weight file in your training script.
     - You can use this file for inference tasks to detect seat belt usage in images or videos.
   
     Example of loading the model:
     python
     from ultralytics import YOLO
     model = YOLO('weights/seatbeltWbest (1).pt')
     

2. *windsheildWbest (2).pt*
   - *Description*: This is the model weight file for detecting windshields in the context of vehicle safety. The model was trained on a similar architecture but for a different task related to safety features.
   - *Usage*: 
     - Similar to the seat belt model, this file can be used for detection tasks related to windshields, if applicable in the project.
   
     Example of loading the model:
     python
     from ultralytics import YOLO
     model = YOLO('weights/windsheildWbest (2).pt')
     

## How to Use These Weights

1. *Loading the Model for Inference*:
   - You can load the weights into the YOLOv8 model for inference by using the YOLO class from the ultralytics library. Here is an example for loading the seatbeltWbest (1).pt model:

   ```python
   from ultralytics import YOLO
   model = YOLO('weights/seatbeltWbest (1).pt')
