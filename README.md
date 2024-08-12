# CIFAR10-Image-Classification
# 🎨 CIFAR-10 Image Classification with PyTorch

![Python](https://img.shields.io/badge/Python-3.x-blue.svg) ![PyTorch](https://img.shields.io/badge/PyTorch-1.x-orange.svg) ![License](https://img.shields.io/badge/License-MIT-green.svg)

Welcome to the CIFAR-10 Image Classification project! This repository contains a Convolutional Neural Network (CNN) implemented in PyTorch, designed to classify images into one of 10 classes.

## 📜 Table of Contents

- [🌟 Introduction](#-introduction)
- [📚 Dataset](#-dataset)
- [🏗️ Model Architecture](#%EF%B8%8F-model-architecture)
- [🔧 Training](#-training)
- [📈 Results](#-results)
- [🚀 How to Use](#-how-to-use)
- [📦 Dependencies](#-dependencies)
- [📬 Contact](#-contact)

## 🌟 Introduction

This project implements a CNN model using PyTorch to classify images from the CIFAR-10 dataset. The goal is to achieve high accuracy in identifying the correct class for each image.

<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:700/1*4ZyX8dTG50oDR6izQoIV3A.png" alt="CIFAR-10 Classes" width="500"/>
</p>

## 📚 Dataset

The CIFAR-10 dataset consists of 60,000 images in 10 classes, with 6,000 images per class. The dataset is divided into 50,000 training images and 10,000 test images.

### 🔍 Dataset Exploration

- **Classes:** Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck.
- **Visualization:** Random images and pixel value distributions across color channels.

<p align="center">
  <img src="https://raw.githubusercontent.com/yourusername/cifar10-image-classification/main/images/sample_images.png" alt="Sample CIFAR-10 Images" width="600"/>
</p>

## 🏗️ Model Architecture

The model architecture includes:

1. **Conv Layer 1**: 3 channels (input), 6 channels (output), 5x5 kernel.
2. **MaxPool Layer 1**: 2x2 kernel.
3. **Conv Layer 2**: 6 channels (input), 16 channels (output), 5x5 kernel.
4. **Fully Connected 1**: 16 * 5 * 5 input, 120 output.
5. **Fully Connected 2**: 120 input, 84 output.
6. **Fully Connected 3**: 84 input, 10 output.

This architecture efficiently processes 32x32 images, extracting features and making predictions.

## 🔧 Training

- **Loss Function:** Cross-Entropy Loss
- **Optimizer:** SGD (Learning Rate: 0.001, Momentum: 0.9)
- **Epochs:** 10

Training was monitored through loss values, and adjustments were made to optimize the model.

## 📈 Results

After training, the model achieved an accuracy of **X%** on the test set. Below is a confusion matrix to visualize the classification performance.

<p align="center">
  <img src="https://raw.githubusercontent.com/yourusername/cifar10-image-classification/main/images/confusion_matrix.png" alt="Confusion Matrix" width="500"/>
</p>

## 🚀 How to Use

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/cifar10-image-classification.git
cd cifar10-image-classification
