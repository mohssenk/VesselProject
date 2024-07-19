# Vessel Project

## Project Overview
The Vessel Project aims to segment retinal blood vessels using a U-net model trained on images from the CHASE, HRF, and DRIVE datasets. The primary objective is to outline all the vessels in retinal images and create corresponding masks.

## Features
Retinal Image Segmentation: Utilizes U-net for segmenting blood vessels in retinal images.
Data Augmentation: Horizontal augmentation applied to increase training data.
Performance Evaluation: Achieves approximately 79% accuracy in vessel segmentation.

## Dataset
Training Data: 73 images (augmented to 146).
Testing Data: 20 images.

## Project Structure
Folders:
  RetinalImages/
-     Test/: Contains original and masked test images.
      Masks/
      Images/
-     Training/: Contains original and masked training images.
      Masks/
      Images/
-     Processed/: Contains processed images.
      Test/
      Train/
-     Processed_cropped/: Contains cropped processed images.
      Test/
      Train/
-     Predicted_masks/: Contains predicted masks of the crops from the 20 test images.
-     Reconstructed_masks/: Contains reconstructed masks from the predicted masks.

## Scripts
- processing_script.ipynb: Initial image processing.
- cropping_processing_script.ipynb: Cropping processed images.
- Model.py: Defines the U-net model.
- model_train.ipynb: Trains the U-net model and saves the best model as unet_best_model.h5.
- reconstructing_processing_script.ipynb: Reconstructs masks from predicted crops.

## Usage
Processing Images:
Run processing_script.ipynb to preprocess the images.

Cropping Images:
Run cropping_processing_script.ipynb to crop the processed images.

Training the Model:
Run model_train.ipynb to train the U-net model. The best model will be saved as unet_best_model.h5.

Reconstructing Masks:
Run reconstructing_processing_script.ipynb to reconstruct the masks from the predicted crops.

## Results
The model achieves an accuracy of approximately 79% when comparing the original masks to the reconstructed masks.

## Credits
This project was inspired by the paper: https://arxiv.org/pdf/1911.09915.
