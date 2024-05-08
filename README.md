# Brain Tumour Detection

This project aims to detect the presence of brain tumors in medical images using deep learning techniques. It utilizes the VGG19 convolutional neural network architecture pre-trained on the ImageNet dataset for feature extraction and binary classification.

## Project Overview

The main components of the project include:

1. **Data Collection**: Medical images containing brain scans are collected from the Brain Tumour Dataset.

2. **Data Augmentation**: Images are augmented using various techniques such as rotation, shifting, shearing, zooming, brightness adjustment, and flipping to increase the dataset size and improve model generalization.

3. **Model Development**: A deep learning model is constructed using the VGG19 architecture as the convolutional base, followed by a fully connected layer with sigmoid activation for binary classification.

4. **Model Training**: The model is trained on the augmented dataset to learn to classify brain scans into two categories: with tumor and without tumor.

5. **Model Evaluation**: The trained model's performance is evaluated on a separate test dataset to assess its accuracy in tumor detection.

6. **Deployment**: The trained model can be deployed as a predictive tool for real-time brain tumor detection in medical applications.

**Note**: 
Adjust the epochs count based on your system specifications.

## Usage

To use the model for predicting brain tumors, follow these steps:

1. **Install Dependencies**: Make sure you have all the required dependencies installed. You can install them using `pip`:
   
   ```bash
   pip install -r requirements.txt

2. **Load Pre-trained Model**: Load the pre-trained model weights using the provided 'brain_tumour.weights.h5' file.

3. **Predict Tumors**: Use the predict_tumor() function to predict whether a brain scan contains a tumor or not.