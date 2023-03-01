# Histopathologic
medical images, binary class classification 

## Dataset
* Number of train samples: 220025
* Number of test samples: 57458
* Image size: 96 * 96 * 3

The task is binary class classificatoin, and our goal is to train a model that can read the medical images and distinguish positive cases from negatives. You can find the full dataset on Kaggle: https://www.kaggle.com/competitions/histopathologic-cancer-detection/overview

## EDA
All images are the same shape, and there are no duplicates. They are ready to be used for training. 

## Model structure
The train dataset is large, so we can use a slightly more complex model.  I built a CNN model with various types of layers, such as Conv2D, MaxPooling, Dropout ... and finally a Dense layer for classification. 

## Results
Our model learned sufficiently after the first epoch but encountered overfitting issues as the training continued. 

## Discussions
Pre-trained models specifically trained for medical images should have much beter results than the naive model in this notebook. Unfortunately, under the scope of this project, I did not investigate those possibilities. 
