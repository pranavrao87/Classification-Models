# Binary and Multiclass Classification using Convolutional Neural Network (CNN)
This repository contains multiple Convolutional Neural Network (CNN) trained on different datasets from waste to pneumonia. 

## Dataset
The dataset used for training and evaluating these CNNs consists of images of various items, divided into two or more classes. All of the datasets were taken off Kaggle.

In the notebooks I pre-process the data since there is usually an uneven amount of images for each class and the training and testing folders. 

In order to get access to the dataset(s) without downloading the entire dataset you need to use the Kaggle API Key and for that you need to create an account. Once you create an account go to your account and click on create a new token.

<img width="467" alt="image" src="https://github.com/pranavrao87/Waste-Classification/assets/108501622/006083b8-f493-4811-b95a-5403b0888bc0">

Then once done with that go to your google colab notebook and upload the key into the local runtime environment

<img width="686" alt="image" src="https://github.com/pranavrao87/Waste-Classification/assets/108501622/3b7b0f17-46db-45a1-9c48-cbdace491af0">

Then the rest of the notebook and code should work.

## Requirements
Python (>=3.6)
TensorFlow (>=2.0)
NumPy
Matplotlib (for visualization)
Google Colab

## Base Model Architecture
The CNN architecture used for this classification task was taken from the CNN explainer website, the TinyVGG model. https://poloclub.github.io/cnn-explainer/

This model consists of a series of convolutional layers followed by max-pooling layers for feature extraction. The extracted features are then flattened and fed into fully connected layers for classification. 

Feel free to experiment with different CNN architectures, hyperparameters, and data augmentation techniques to improve the model's performance.



