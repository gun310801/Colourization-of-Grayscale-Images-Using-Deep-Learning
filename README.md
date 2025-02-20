# Grayscale Image Colorization using Deep Learning

## Overview

This project implements a deep learning model to automatically colorize grayscale images. The model utilizes convolutional neural networks (CNNs) to predict the colors of a monochrome image and produce a colored output. This technology can be applied to various applications, including enhancing old films and pictures and improving face detection in biometric systems.
## Introduction

### Abstract

Colorization is the process of adding shades of color to a monochrome picture or film. Traditionally, this process involved significant manual effort. This project aims to automate this process using deep learning technology, specifically convolutional neural networks (CNNs), to develop a code that can predict the colors of a monochrome image and colorize it automatically.

### Background

A colored image stores color information for each pixel (e.g., Red, Green, and Blue values in the RGB color space), whereas a grayscale image stores only intensity information. Converting a grayscale image to color involves generating the missing color information. This project uses a CNN to learn the mapping between grayscale intensities and color values.

## Methodology

### Method Used

The project uses a Convolutional Neural Network (CNN) to learn the colorization process. Key aspects of the methodology include:

1.  **CNN Architecture:**  The CNN model is constructed with multiple layers using Keras. These layers typically include Conv2D (Convolutional Layer) and Conv2DTranspose (Deconvolutional Layer) with ReLU activation functions.

2.  **Color Space:** The images are converted into the LAB color space (L for Lightness, A for Green-Magenta, and B for Blue-Yellow). The model takes the grayscale image as the L channel input and predicts the A and B channels to generate a colored image.

3.  **Training:**  The model is trained on a dataset of color images. The grayscale version of the color images is used as input, and the original color image is used as the target output.

4.  **Key Steps**
    1.  Import the grayscale images dataset as a NumPy array.
    2.  Convert the grayscale images into the LAB format.
    3.  Divide the dataset into a training set and a test set.
    4.  Create a Convolutional Neural Network using multiple layers in Keras.
    5.  Use the Adam Optimizer and loss function to see the loss while training the model.
    6.  Check for errors using a sample image.
    7.  Train the model against a number of epochs.
    8.  Predict the colorized output of input test images.

### Algorithm

The project utilizes the following algorithm to colorize grayscale images:

*   Conv2D layer with a relu activation function
*   Conv2D layer with a relu activation function
*   Conv2DTranspose layer with a relu activation function
*   Conv2DTranspose layer with a relu activation function

### Applications

*   **Conversion of Old Videography:** Colorize old black and white videos.
*   **Detailed Image Reconstruction:** Enhance the visual appeal of grayscale images.
*   **Improved Interpretation of Modern Grayscale Images:** Improve images from CCTV cameras, astronomical photography, or electron microscopy.
