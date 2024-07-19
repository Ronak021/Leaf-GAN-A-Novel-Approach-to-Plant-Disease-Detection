# Leaf GAN: A Novel Approach to Plant Disease Detection

## Team Members
- Ronak Chauhan (21BCE038)
- Vansh Diyora (21BCE060)
- Naimish Gajjar (21BCE069)


## Overview
Leaf GAN is an innovative project aimed at detecting plant diseases using deep learning techniques. This project focuses on identifying three specific classes of leaf conditions: healthy, septoria, and stripe rust, using a novel Indian-origin dataset.

## Problem It Solves
Leaf GAN addresses the critical issue of plant disease detection in agriculture, focusing on early identification and classification of diseases to prevent crop loss, optimize resource use, and enhance agricultural productivity.

## Main Outcomes
1. **Accurate Disease Identification**: Classifies leaf images into healthy, septoria, and stripe rust categories.
2. **Advanced Model Techniques**: Utilizes U-Net with pre-trained networks and Grad-CAM for improved accuracy and interpretability.
3. **Enhanced Dataset**: Uses augmentation and integration with the ImageNet dataset to improve model robustness and diversity.

## Dataset Description
The dataset comprises a total of 407 images categorized into three distinct classes:
- **Healthy**: 102 images depicting healthy leaves.
- **Septoria**: 97 images of leaves affected by septoria.
- **Stripe Rust**: 208 images of leaves afflicted with stripe rust.

### Novelty
This dataset is pioneering in plant pathology and agriculture, offering meticulously curated images representing leaf conditions prevalent in Indian agriculture. It addresses the unique needs of Indian farmers and includes diseases like septoria and stripe rust, making it a valuable tool for developing targeted solutions to improve crop health and productivity in India and similar agricultural regions worldwide.

## Proposed Algorithm
### Dataset Preparation
1. **Resizing**: Resize original leaf images to 500x500 pixels.
2. **Augmentation**: Generate eight new images from each original image, resulting in 3663 images, labeled '0'.
3. **Partitioning**: Resize original images to 1500x1500 pixels and partition into nine 500x500 images, labeled '1'.
4. **ImageNet Dataset Integration**: Integrate 3663 images from ImageNet, partitioned into nine equivalent images, labeled '2'.

### Model Training
1. **U-Net with Pretrained Network (VGG16)**
   - Benefits from learned feature representations, enhancing segmentation performance.
2. **U-Net from Scratch**
   - Trains from random initialization, learning task-specific features.
3. **Grad-CAM**
   - Visualizes and interprets model decisions, aiding validation and interpretation.

## Results
1. **Output with Raw Image as Input**: Model predictions on raw images.
2. **Output with Preprocessing and Applying Grad-CAM**: Predictions with Grad-CAM visualizations on preprocessed images.

## Installation and Usage
### Prerequisites
- Python 3.x
- Jupyter Notebook


