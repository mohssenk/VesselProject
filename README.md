# Vessel Project

## Project Overview
The Vessel Project aims to segment retinal blood vessels using a U-net model trained on images from the CHASE, HRF, and DRIVE datasets. The primary objective is to outline all the vessels in retinal images and create corresponding masks.

The scripts are designed to be run in Google Collab.

## Features
Retinal Image Segmentation: Utilizes U-net for segmenting blood vessels in retinal images.

Data Augmentation: Horizontal augmentation applied to increase training data.

Performance Evaluation: Achieves approximately 79% accuracy in vessel segmentation.

U-net can be viewed [here](https://drive.google.com/file/d/1ZoxYWVA33N-eV8x7h9zJHn3BUdWdQYUn/view?usp=sharing)

## Dataset
- Training Data: 73 images (augmented to 146).
- Testing Data: 20 images.
- Training Crops: 24674 crops.
- Testing Crops: 3380 crops.

## Project Sections (can be viewed through Google Collab)

[Part 1: Initial processing](https://colab.research.google.com/drive/1VMovHh_UP_c6gzeyY7ccjO_zObRFsySk#scrollTo=3sa4X_XXOnw0)

[Part 2: Creating the dataset using images](https://colab.research.google.com/drive/1BwMzLDErF3z0Uac-7mNmGYKC3cW1anj4#scrollTo=9gVFZD1sQ-0U)

[Part 3: Training the U-net](https://colab.research.google.com/drive/1o7xiHB1q73OHhJY8LWF8fRgsLucOCZwV#scrollTo=3AJA1vFl7-2S)

[Part 4: Reconstruction - seeing the results](https://colab.research.google.com/drive/1mCgdzgRPaw19VW8F83vSjl2W9cgOs22G#scrollTo=rBjJ_1DZN4Dy)

## Results
The model achieves an accuracy of approximately 79% when comparing the original masks to the reconstructed masks.
The following is an example result:
![WhatsApp Image 2024-07-16 at 17 45 35_a8dc3c2e](https://github.com/user-attachments/assets/56aea650-e60e-479c-8caa-9140075e8c85)

# Data
- [RetinalImages](https://drive.google.com/drive/u/0/folders/1Rpvv94i4UVRSjpQh8Oz4z9uUspljQzC0)/
  - Test/: Contains original and masked test images.
  - Training/: Contains original and masked training images.
  - Processed/: Contains processed images.
  - Processed_cropped/: Contains cropped processed images.
  - Predicted_masks/: Contains predicted masks of the crops from the 20 test images.
  - Reconstructed_masks/: Contains reconstructed masks from the predicted masks.

## Credits
This project was based off the paper: https://arxiv.org/pdf/1911.09915.
