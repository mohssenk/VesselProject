# Vessel Project

## Project Overview
The Vessel Project aims to segment retinal blood vessels using a U-net model trained on images from the CHASE, HRF, and DRIVE datasets. The primary objective is to outline all the vessels in retinal images and create corresponding masks.

The scripts are designed to be run in Google Collab.

## Features
Retinal Image Segmentation: Utilizes U-net for segmenting blood vessels in retinal images.

Data Augmentation: Horizontal augmentation applied to increase training data.

Performance Evaluation: Achieves approximately 79% accuracy in vessel segmentation.

## Dataset
- Training Data: 73 images (augmented to 146).
- Testing Data: 20 images.
- Training Crops: 24674 crops.
- Testing Crops: 3380 crops.

Due to space, the images and their processed counterparts will be uploaded, but none of the crops will be uploaded, but can be easily generated. There are 169 crops per image.

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
The following is an example result:
![WhatsApp Image 2024-07-16 at 17 45 35_a8dc3c2e](https://github.com/user-attachments/assets/56aea650-e60e-479c-8caa-9140075e8c85)


## Credits
This project was based off the paper: https://arxiv.org/pdf/1911.09915.
