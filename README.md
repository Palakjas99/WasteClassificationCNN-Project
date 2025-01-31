# CNN Model for Plastic waste Classification
# Project Overview
This project focuses on using a Convolutional Neural Network (CNN) to identify and categorize plastic waste from images. The goal is to automate the process of classifying various types of plastic waste, enabling more efficient recycling processes and better waste management practices.
# Week 1
# Dataset Link:
https://www.kaggle.com/datasets/techsash/waste-classification-data/data
# Features
- Classify plastic waste images into categories (e.g., PET, PVC, HDPE, etc.)
- Provide a trained CNN model for waste classification
- Image preprocessing and augmentation for better performance
# Week 2
In Week 2, we have enhanced our deep learning model for waste classification by making significant updates to the Week 1 code. Below are the key improvements and additions:

1. Data Visualization Enhancement:
   
Introduced a grid visualization of random images from the dataset using plt.subplot().
The images are randomly selected and labeled, helping us understand dataset variations.

2. CNN Model Architecture Expansion:

Added a third convolutional layer (128 filters) to capture more complex image features.
Increased model depth to improve accuracy.
Implemented Dropout layers (0.5 rate) in the dense layers to prevent overfitting.

3. Training and Testing Generators:
   
Used ImageDataGenerator.flow_from_directory() to dynamically load images from the dataset.
Ensured RGB conversion and maintained 224x224 resolution.
Configured class_mode='categorical' for multi-class classification.

4. Model Training & Validation:

Trained the model for 10 epochs using the model.fit() function.
Added validation_data=test_generator to track validation performance.
