# 🎨 CIFAR-10 Image Classification with PyTorch

![Python](https://img.shields.io/badge/Python-3.x-blue.svg) ![PyTorch](https://img.shields.io/badge/PyTorch-1.x-orange.svg) ![GoogleColaboratory](https://img.shields.io/badge/Colab-1.x-yellow.svg) 

Welcome to the CIFAR-10 Image Classification project! This repository contains a Convolutional Neural Network (CNN) implemented in PyTorch, designed to classify images into one of 10 classes.

## 📜 Table of Contents

- [📚 Dataset](#-dataset)
- [🏗️ Model Architecture](#%EF%B8%8F-model-architecture)
- [🔧 Training](#-training)
- [📦 Dependencies](#-dependencies)
- [📬 Contact](#-contact)

## 📚 Dataset

This project implements a CNN model using PyTorch to classify images from the CIFAR-10 dataset. The goal is to achieve high accuracy in identifying the correct class for each image.
The CIFAR-10 dataset consists of 60,000 images in 10 classes, with 6,000 images per class. The dataset is divided into 50,000 training images and 10,000 test images.
<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:4800/format:webp/1*PikwjA1WEmFNX-kYE24QYA.png" alt="CIFAR-10 Classes" width="500"/>
</p>

### 🔍 Dataset Exploration

- **Classes:** Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, Truck.
- **Visualization:** Random images and pixel value distributions across color channels.

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

Training was monitored through loss values, and adjustments were made to optimize the model. After training, the model achieved an accuracy of **62.04%** on the test set. Below is a confusion matrix to visualize the classification performance.
<p align="center">
  <img src="https://raw.githubusercontent.com/zhordiffallah/cifar10-image-classification/main/images/confusion_matrix.png" alt="Sample CIFAR-10 Images" width="600"/>
</p>
## 📦 Dependencies
- Python 3.x
- PyTorch
- NumPy
- Matplotlib
- Seaborn (optional for extra visualizations)

## 📬 Contact
Feel free to reach out if you have any questions or suggestions!
📧 Email: zhor.diffallah@gmail.com
💼 LinkedIn: Zhor Diffallah
