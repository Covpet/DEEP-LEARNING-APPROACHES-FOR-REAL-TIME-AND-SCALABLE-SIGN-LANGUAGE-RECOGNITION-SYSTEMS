### DEEP LEARNING APPROACHES FOR REAL TIME AND SCALABLE SIGN LANGUAGE RECOGNITION SYSTEMS

## Overview
This repository contains the implementation of a real-time, scalable sign language recognition system using Convolutional Neural Networks (CNNs). The system identifies hand gestures for alphabets (A-Z) and numbers (0-9) to bridge communication barriers for individuals with hearing and speech impairments.

## Features
- High accuracy (96% on training data, 94% on validation data)
- Automated feature extraction using CNNs
- Scalable to larger datasets and adaptable for real-time use

  
## Abstract
Sign language is essential for individuals with hearing and speech impairments. This project utilizes CNNs to classify gestures into letters and numbers. The system achieved high accuracy and demonstrates potential for real-world applications.

## Project Motivation
The limited understanding of sign language in broader society restricts effective communication. This project aims to:

- Bridge the gap between the hearing-impaired community and society.
- Provide an automated and scalable solution using deep learning.
  
## Dataset Overview
- Source: ASL Dataset on Kaggle
- Classes: 36 (26 letters, 10 digits)
# Images per class
- Training: 60
- Validation: 10
# Preprocessing Steps:
- Resizing to 224x224 pixels
- Normalization (scaling pixel values to [0, 1])
- Augmentation (rotation, flipping, zooming)

## Model Architecture
The CNN model comprises:
- Input Layer: Images resized to 224x224 with three RGB channels.
- Convolutional Layers: Two layers with 32 and 64 filters (3x3 kernels).
- Pooling Layers: Max-pooling to reduce spatial dimensions.
- Dropout Layer: Regularization with a dropout rate of 50%.
# Fully Connected Layers:
- Dense layer with 128 neurons.
- Output layer with 36 neurons (softmax activation).
