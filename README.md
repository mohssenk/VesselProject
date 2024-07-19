# Vessel Project

## Project Overview
The Vessel Project aims to segment retinal blood vessels using a U-net model trained on images from the CHASE, HRF, and DRIVE datasets. The primary objective is to outline all the vessels in retinal images and create corresponding masks.

The scripts are designed to be run in Google Collab.

## Features
Retinal Image Segmentation: Utilizes U-net for segmenting blood vessels in retinal images.

Data Augmentation: Horizontal augmentation applied to increase training data.

Performance Evaluation: Achieves approximately 79% accuracy in vessel segmentation.

U-net can be viewed ![here](https://drive.google.com/file/d/1ZoxYWVA33N-eV8x7h9zJHn3BUdWdQYUn/view?usp=sharing)

## Dataset
- Training Data: 73 images (augmented to 146).
- Testing Data: 20 images.
- Training Crops: 24674 crops.
- Testing Crops: 3380 crops.

## Project Sections (can be viewed through Google Collab)

![Part 1](https://drive.google.com/file/d/1VMovHh_UP_c6gzeyY7ccjO_zObRFsySk/view?usp=sharing)

![Part 2](https://drive.google.com/file/d/1BwMzLDErF3z0Uac-7mNmGYKC3cW1anj4/view?usp=sharing)

![Part 3](https://drive.google.com/file/d/1o7xiHB1q73OHhJY8LWF8fRgsLucOCZwV/view?usp=sharing)

![Part 4](https://drive.google.com/file/d/1mCgdzgRPaw19VW8F83vSjl2W9cgOs22G/view?usp=sharing)

## Results
The model achieves an accuracy of approximately 79% when comparing the original masks to the reconstructed masks.
The following is an example result:
![WhatsApp Image 2024-07-16 at 17 45 35_a8dc3c2e](https://github.com/user-attachments/assets/56aea650-e60e-479c-8caa-9140075e8c85)


## Credits
This project was based off the paper: https://arxiv.org/pdf/1911.09915.
