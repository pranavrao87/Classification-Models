# Organic vs. Recyclable Waste Classification using Convolutional Neural Network (CNN)
This repository contains a simple Convolutional Neural Network (CNN) designed to differentiate between organic and recyclable waste items. The CNN model is trained on a labeled dataset of waste images and is capable of classifying new waste items into one of these two categories. As of now it is roughly 85% accurate 

## Dataset
The dataset used for training and evaluating the CNN consists of images of various waste items, divided into two classes: organic (O) and recyclable (R). It was gotten of Kaggle, https://www.kaggle.com/datasets/techsash/waste-classification-data.

In the notebook I pre-process the data since there is an uneven amount of images for each class so I only use 880 images for both classes for training and 220 images for both classes for testing. 

In order to get access to the data without downloading the entire dataset you need to use the Kaggle API Key and for that you need to create an account. Once you create an account go to your account and click on create a new token.

<img width="467" alt="image" src="https://github.com/pranavrao87/Waste-Classification/assets/108501622/006083b8-f493-4811-b95a-5403b0888bc0">

Then once done with that go to your google colab notebook and upload the key into the local runtime environment

<img width="686" alt="image" src="https://github.com/pranavrao87/Waste-Classification/assets/108501622/3b7b0f17-46db-45a1-9c48-cbdace491af0">

Then the rest of the notebook and code should work.

The dataset structure should look like this:

      DATASET
      |
      | --- TRAIN
            |-- O
            |-- R
      |
      | --- TEST
            |-- O
            |-- R
      |
      |
      EXTRA
      |-- O
      |-- R

The Extra folder is for all the extra images that weren't used in order to provide the model with an even amount of training and testing images for both types of data. It is also placed outside of the main DATASET folder intentionally in order to avoid any confusion.

## Requirements
Python (>=3.6)
TensorFlow (>=2.0)
NumPy
Matplotlib (for visualization)
Gooogle Colab

## Base Model Architecture
The CNN architecture used for this classification task was taken from the CNN explainer website, the TinyVGG model. https://poloclub.github.io/cnn-explainer/

This model consists of a series of convolutional layers followed by max-pooling layers for feature extraction. The extracted features are then flattened and fed into fully connected layers for classification. 

Feel free to experiment with different CNN architectures, hyperparameters, and data augmentation techniques to improve the model's performance.



