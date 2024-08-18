# Deep Autoencoders for MNIST and FMNIST: Analysis and Denoising

## Overview

This repository contains the code and results for Project 1 in our Data Science and Engineering course, focusing on the implementation and evaluation of deep autoencoders using the MNIST and FMNIST datasets. The primary objectives are to explore different autoencoder architectures, regularization techniques, and their impacts on performance, including image denoising capabilities.

**Credit:**
The implementation is based on tasks provided by Pablo M. Olmos.

**Completed by:**
- **María Ángeles Magro Garrote** - [mariamagro](https://github.com/mariamagro)
- **Marina Gómez Rey** - [MarinaGRey](https://github.com/MarinaGRey)
- **Ángela Durán**

## Project Description

### Abstract

This project investigates deep autoencoder models on MNIST and FMNIST datasets, comparing 3-layer and 5-layer architectures with varying projected dimensions (15, 30, 50, 100). We also explore Lasso and Dropout regularization techniques and evaluate the best performing architecture as a denoising autoencoder. Performance is assessed using Peak Signal-to-Noise Ratio (PSNR), with visual comparisons to measure the effectiveness of the denoising process.

### Introduction

Autoencoders are neural networks designed to learn compressed representations of input data. This project focuses on deep autoencoders for tasks such as image reconstruction and denoising. We assess the impact of different network architectures and regularization techniques, specifically:

- **Lasso Regularization**: Penalizes the absolute values of network weights to encourage sparsity.
- **Dropout Regularization**: Randomly deactivates neurons during training to prevent overfitting.

We also explore denoising autoencoders, which aim to reconstruct clean images from noisy inputs by introducing Gaussian noise and evaluating the denoising performance using PSNR.

### Code & Results

The code is implemented in the Jupyter Notebook `Code.ipynb`, and the results are documented in `Report.pdf`. Here’s a summary of the key parameters and configurations used:

- **Input Size**: 784 pixels (28x28 images)
- **Number of Epochs**: 10
- **Batch Size**: 128
- **Learning Rate**: 0.001
- **Lasso Regularization**: 0.00001
- **Noise Variances**: [0.1, 0.25, 0.5, 0.75, 1]

#### Regularization Techniques

- **Dropout Autoencoder**: Utilizes dropout layers in both encoder and decoder.
- **Lasso Autoencoder**: Incorporates L1 regularization directly into the loss function.

## Files

- `Code.ipynb`: Jupyter Notebook containing the implementation of autoencoders, training procedures, and evaluations.
- `Report.pdf`: Comprehensive report detailing the methodologies, experiments, and results.
