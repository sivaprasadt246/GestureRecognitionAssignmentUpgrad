# Gesture-Recognition-Deep-Learning 
Project to recognize hand gesture using neural networks.

## Team
 Siva Prasad Thota & Sukumar Moharana.
 
## Problem Statement 
We need to develop a cool feature in the smart-TV that can recognise five different gestures performed by the user which will help users control the TV without using a remote.
The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:

- Thumbs up:  Increase the volume
- Thumbs down: Decrease the volume
- Left swipe: 'Jump' backwards 10 seconds
- Right swipe: 'Jump' forward 10 seconds  
- Stop: Pause the movie

## Understanding the Dataset
The training data consists of a few hundred videos categorised into one of the five classes. Each video (typically 2-3 seconds long) is divided into a sequence of 30 frames(images). These videos have been recorded by various people performing one of the five gestures in front of a webcam - similar to what the smart TV will use.

Our task is to train different models on the 'train' folder to predict the action performed in each sequence or video and which performs well on the 'val' folder as well.  

Dataset available @ https://drive.google.com/drive/folders/1rU_r0r4SStCiICTEslgjRrmNFAhx_-ON

## Model Overview
We will be using two types of architectures for analysing videos using deep learning 
1.	CNN + RNN architecture 
2.	3D Convolutional Neural Networks (Conv3D)

### Data pre-processing 
1.	Deciding on number of images to be taken per video/sequence
2.	Resizing and cropping the images
3.	Normalizing the images

### Data Generators
In this project, we have written our own batch data generator. After iterating over the chosen batch size, we have iterated over the remaining data points which were left after full batches

## Technologies Used
- Keras
- TensorFlow
- Python
- Pandas, Numpy, Matplotlib

## Conclusion
