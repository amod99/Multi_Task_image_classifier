# Multi_Task_image_classifier
This is a baseline CNN implementation for multi label image classification for this kaggle competition : https://www.kaggle.com/c/severstal-steel-defect-detection 

# Data pre-processing 

We derive multiple labels for individual images from labelled data set provided seperately in the competition. 
Implemented Multilabelbinarizer to create one hot encoding for multi label images.
Images are already in standard shape. We pass in np array of images after scaling every pixel value by 255. 

# Image Classification
There are 2 tasks described in the competition : 
1. Defect classification
2. Defect location

Here we are presenting solution to task #1. CNN model architecture is inspired from coursera material and this blog post : 
https://www.analyticsvidhya.com/blog/2019/04/build-first-multi-label-image-classification-model-python/

There are 4 different defects. Some of the images have 1 or many defects while some images dont have defects at all. 
CNN architecture comprises of :
1. Zeropadding
2. multiple Conv2D layers with relu activation
3. Dropout layer

Since this is a multi label classification task we use sigmoid activation for the final dense layer. 
Accuracy on test set for this baseline model is 72%.


