# Emotion Classification with CNNs
## Overview
This project implements emotion classification on the CK+ dataset using two Convolutional Neural Network (CNN) models. The goal is to classify 8 emotions: Anger, Disgust, Fear, Happiness, Sadness, Surprise, Neutral, and Contempt. Two models (a simple CNN and a deeper CNN) are trained, evaluated, and compared.

## Dataset
* ***CK+ Dataset:*** Contains 981 grayscale images (48x48 pixels) with 8 emotion labels.
* Preprocessing: Reduced Neutral class samples to 100 to balance the dataset, normalized pixel values, and split into train/validation/test sets (test set: 89 samples).
* You can access the dataset [here](https://www.kaggle.com/datasets/davilsena/ckdataset).

## Models
1. **Simple Model:** 2 convolutional layers (32, 64 filters), Dropout (0.3), Dense (64 units), trained for 30 epochs.
2. **Deep Model:** 3 convolutional layers (64, 128, 256 filters), L2 regularization, Dropout (0.5), Dense (128 units), trained for 50 epochs.
