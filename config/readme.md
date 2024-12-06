# Configuration Files - Seat Belt Detection Project

This folder contains the configuration files for training and fine-tuning YOLOv8 models for the Seat Belt Detection project. There are two primary configuration files:

## Folder Structure and Files

### *Model Configuration Files*

1. *custom (2).yaml*  
   - *Description*: This is the primary configuration file for training the YOLOv8 model. It includes a mix of default and custom settings to optimize the model for seat belt detection tasks. The configuration defines the architecture, hyperparameters, and dataset specifics.
   
   - *Key Parameters*:  
     - *batch_size*: Defines the number of images processed in one batch during training.
     - *epochs*: Specifies the number of training epochs.
     - *learning_rate*: Learning rate for the optimizer.
     - *input_size*: Image input size for the model.
     - *optimizer*: Optimizer settings (e.g., Adam, SGD).
     - *anchors*: Custom anchor box values for better bounding box prediction.
     - *classes*: Class labels, such as "Seat Belt" and "No Seat Belt".

2. *customyolov8n (1).yaml*  
   - *Description*: This configuration is specifically tailored for the YOLOv8 model with depth-wise convolution (dw conv) architecture. The dw conv architecture reduces model size and improves computational efficiency without sacrificing performance.
   
   - *Key Parameters*:  
     - *depthwise_convolution*: Enables depth-wise convolutions for faster processing.
     - *width_multiple*: Adjusts the width of the model layers.
     - *depth_multiple*: Adjusts the depth of the model layers for balancing performance and speed.
     - *pretrained_weights*: Path to the pretrained weights file (yolov8n.pt).

### *How to Use These Configuration Files*

1. *For Custom Model Training*:
   - Use custom (2).yaml to train the YOLOv8 model with the standard architecture.  
   - You can modify hyperparameters like batch size, learning rate, and the number of epochs based on your training environment.

   To start training with this configuration:
   ```bash
   python train.py --cfg config/custom\ (2).yaml (as mentioned in the code folder train_yolov8_seatbelt.ipynb)
