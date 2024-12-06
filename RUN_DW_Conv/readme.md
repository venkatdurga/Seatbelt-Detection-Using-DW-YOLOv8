# Training Results - Seat Belt Detection Project

This folder contains the results and outputs generated during the training of the Seat Belt Detection model. The model was trained using the YOLOv8 architecture and evaluated using various metrics. Below is a breakdown of the files in this directory:

## Folder Structure and Files

### *Training Results*  
- *F1_curve.png*  
  - The F1 score curve over training epochs, visualizing the balance between precision and recall during training.

- *PR_curve.png*  
  - Precision-Recall curve for model evaluation, showing the trade-off between precision and recall.

- *P_curve.png*  
  - Precision curve, plotting the model's precision during training.

- *R_curve.png*  
  - Recall curve, showing how recall evolved throughout the training process.

- *args.yaml*  
  - A YAML configuration file containing hyperparameters and training settings used during the model training.

- *confusion_matrix.png*  
  - The confusion matrix for model performance on the validation set, visualizing true positives, false positives, true negatives, and false negatives.

- *confusion_matrix_normalized.png*  
  - Normalized version of the confusion matrix, representing the percentage of correct classifications.

- *events.out.tfevents.1714199849.6bb30cf13726.1111.0*  
  - TensorFlow event file containing logs related to training metrics, such as loss and accuracy over time.

- *labels.jpg*  
  - A visual representation of the dataset labels used for training.

- *labels_correlogram.jpg*  
  - Correlogram (correlation matrix) showing the relationships between various class labels.

- *predictions.json*  
  - A JSON file containing the model’s predictions during training.

- *readme.md*  
  - This README file, explaining the contents of the train folder.

- *results.csv*  
  - A CSV file summarizing the model's performance metrics across training epochs.

- *results.png*  
  - A visual summary of the training results, typically showing the loss and accuracy curves.

- *train_batch0.jpg, train_batch1.jpg, train_batch2.jpg*  
  - Images from the training batches showing the input data during training.

- *val_batch0_labels.jpg, val_batch0_pred.jpg, val_batch1_labels.jpg, val_batch1_pred.jpg*  
  - Images showing the labels and predictions for the validation batches.

- *weights.zip*  
  - Compressed file containing the trained weights for the model after training.

### *Pretrained Model*
- *yolov8n.pt*  
  - The pretrained YOLOv8 model file used as the base for training the Seat Belt Detection model.

## How to Use This Folder

1. *Model Weights*:  
   - To continue training or fine-tune the model, use the weights.zip file. You can extract it and load the weights into your YOLOv8 model.

   ```bash
   unzip weights.zip
