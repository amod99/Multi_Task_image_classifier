# Multi_Task_image_classifier
This is a baseline CNN implementation for multi label image classification for this kaggle competition : https://www.kaggle.com/c/severstal-steel-defect-detection 

# Data pre-processing 

We derive multiple labels for individual images from labelled data set provided seperately in the competition. 
Implemented Multilabelbinarizer to create one hot encoding for multi label images.
There are 2 tasks described in the competition : 
1. Defect classification
2. Defect location

Here we are presenting solution to task #1. CNN model architecture is inspired from coursera material and this blog post : 
https://www.analyticsvidhya.com/blog/2019/04/build-first-multi-label-image-classification-model-python/
