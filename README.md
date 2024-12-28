# Eye Location Detection Project

## Introduction
This project aims to develop a convolutional neural network (CNN) model to detect eye positions in grayscale images. Using the BioID Face Database, the model is trained to identify and predict the coordinates of eyes in unseen images.

## Dataset Description
The dataset consists of 499 black and white images (PGM format), each annotated with the locations of the left and right eyes. These annotations are utilized to train and validate the model's performance.

## Objective
The primary goal of this project is to accurately detect eye positions in black and white facial images, which could be used in applications such as biometric identification and facial recognition systems.

## Methodology

### Data Loading
- Images are loaded using the PIL library and preprocessed to grayscale to standardize input for the CNN.
- A custom `Dataset` class is implemented using PyTorch to handle image loading and transforming operations.

### Model Architecture
- The CNN consists of two convolutional layers followed by max pooling and fully connected layers.
- The model outputs four values representing the coordinates of the left and right eyes.

### Training
- The model is trained using a mean squared error loss function and the Adam optimizer.
- Data is split into 80% training and 20% testing to evaluate model performance.

## Requirements
To run this project, the following libraries are needed:
- Python 3.8
- PyTorch
- torchvision
- PIL
- numpy
- matplotlib

## Usage
Detailed instructions on how to set up and run the project, including how to train the model and make predictions on new images.

## Results
The training process results in decreasing loss over epochs, demonstrating learning. The model's performance can be validated against the test set and through visual inspections of predicted versus actual eye coordinates.

## Contributors
- Zhenyuan Ni

## Example Prediction
After training, the model can be used to predict eye positions in new images. An example usage is shown in the code snippet where the model predicts eye locations for a given image, comparing it against the actual annotated coordinates.

