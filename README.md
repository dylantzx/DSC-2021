# DSC-2021

## Description 
The Data Science Competition (DSC) is a one-week long competition that requires participants to produce a Model using Computer Vision techniques that:
1. Should be able to count the number of acumen chips using in the image
2. Locate and recognize handwrittings
3. Detect for anomalies of the acumen chips (Double Stacking and Black Dots) in the images

## Team's Approach
As part of the team's learning process, we have explored the traditional OpenCV techniques using Image processing for Object detection. We experimented with Bilateral Filtering, Gaussian Blur Filtering, Adaptive thresholding, Canny-Edge Detector etc. then used the contour to detect and count the acumen chips. However, as there are many factors affecting the reliability of the results such as lighting, touching objects, clarity of image etc. the team has decided to use a learning-based approach.

The team used YOLOv4 Darknet, an open-sourced Neural Network framework and was able to detect most of the acumen chips across the validation and test images. However, we were unable to complete the implementation of the object counting code and were not able to successfully detect all the anomalies.

Using the MNIST Dataset and Tensorflow, we created a CNN Classification model for the local digit classification. To locate the handwriting, our group annotated the dataset, drew bounding boxes around the handwritten digits in the images and trained the YoloV4 Object Detection model using the dataset. Unfortunately, the approach failed and our model failed to detect the handwritings.

## To work on
1. Complete the implementation of object counting
2. Use data augmentation techniques to increase the data on anomalies
3. Work on locating the handwritings.

## Organizers
NUS Statistics Society and HP
