# U-Net Image Segmentation with PyTorch

## Overview

This project implements a U-Net convolutional neural network using PyTorch for image segmentation. It uses the Oxford-IIIT Pet dataset to train a model that predicts segmentation masks for pet images.

The notebook also demonstrates convolution and transposed convolution operations, image preprocessing, dataset preparation, model training, and prediction visualization.

## Features

- **Convolution Operations:** Implement 2D convolution and transposed convolution using NumPy and PyTorch.
- **Dataset Preparation:** Download, extract, and inspect the Oxford-IIIT Pet dataset.
- **Image and Mask Processing:** Load pet images and their corresponding segmentation masks, resize them, and prepare them for training.
- **U-Net Architecture:** Build an encoder-decoder convolutional neural network with skip connections.
- **Model Training:** Train the network using binary cross-entropy loss and the Adam optimizer.
- **Training Visualization:** Plot the training loss to observe model performance during training.
- **Prediction Visualization:** Compare the input images, predicted segmentation masks, and ground-truth masks.

## Technologies Used

- Python
- PyTorch and Torchvision
- NumPy
- OpenCV
- Matplotlib
- Pillow (PIL)
- Kaggle API
- Jupyter Notebook

## Dataset

This project uses the **Oxford-IIIT Pet Dataset**, which contains pet images and corresponding trimap segmentation annotations.

The notebook prepares the images and masks for model training by resizing them to 128 × 128 pixels.

## Model Architecture

U-Net is an encoder-decoder convolutional neural network designed for image segmentation.

- **Encoder:** Extracts features from images through convolutional blocks and downsampling.
- **Bottleneck:** Processes the extracted high-level features.
- **Decoder:** Upsamples feature maps to recover spatial resolution.
- **Skip Connections:** Transfer features from the encoder to the decoder to help preserve spatial information.
- **Output Layer:** Produces a predicted segmentation mask.

## Training Process

The notebook includes the following steps:

1. Prepare the dataset and segmentation masks.
2. Create a custom PyTorch dataset class.
3. Apply image and mask transformations.
4. Create data loaders for training and testing.
5. Initialize the U-Net model.
6. Configure binary cross-entropy loss and the Adam optimizer.
7. Train the model and visualize the loss.
8. Evaluate predictions visually against the ground-truth masks.

## Learning Objectives

This project explores convolutional neural networks, image segmentation, encoder-decoder architectures, skip connections, custom PyTorch datasets, model optimization, and visual evaluation of segmentation predictions.

## Notes

- A working Kaggle API configuration is required for the dataset download steps.
- The notebook uses GPU acceleration when CUDA is available and otherwise falls back to the CPU.
- Training time depends on the available hardware and dataset size.
- Review dataset paths and dependencies before running the notebook in a new environment.

## Author

**Seyed Amirhossein Mirpour**

Computer Engineering Student | Machine Learning and Deep Learning

---

This project is intended for educational purposes and practical exploration of deep learning-based image segmentation.
