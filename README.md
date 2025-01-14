# Handwritten Digit Classification Using PyTorch

This project implements a neural network for classifying handwritten digits from the MNIST dataset. It includes data preprocessing, model training, validation, and testing, as well as visualizations for performance evaluation.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Results](#results)
- [Acknowledgments](#acknowledgments)

## Overview
The project uses PyTorch to build a multi-layer perceptron (MLP) for classifying digits (0-9). The MNIST dataset is used as the benchmark, and the implementation includes data augmentation, model checkpointing, and performance visualization.

## Features
- Data preprocessing with augmentation (random rotations, random cropping, normalization).
- Train-validation split for better model evaluation.
- Multi-layer perceptron (MLP) with two hidden layers.
- Training with Adam optimizer and Cross-Entropy Loss.
- Model checkpointing based on validation loss.
- Performance visualization: training/validation losses and accuracies.

## Requirements
- Python 3.7+
- PyTorch 1.9+
- torchvision
- matplotlib
- numpy

## Setup
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Run the script to train the model:
   ```bash
   python train_model.py
   ```
   - The script will train the MLP on the MNIST dataset, validate its performance, and save the best model.

2. Evaluate the model on the test dataset:
   ```bash
   python test_model.py
   ```
   - The test loss and accuracy will be displayed.

3. Visualize training and validation performance:
   - Loss and accuracy plots are generated to analyze the model's learning curve.

## Results
- **Training Accuracy**: ~90.40%
- **Validation Accuracy**: ~90.02%
- **Test Accuracy**: ~90.24%

Loss and accuracy trends across epochs are visualized in the generated plots.

## Acknowledgments
- [PyTorch](https://pytorch.org/) for the deep learning framework.
- [MNIST Dataset](http://yann.lecun.com/exdb/mnist/) for the benchmark dataset.
