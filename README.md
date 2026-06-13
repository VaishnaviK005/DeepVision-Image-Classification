# DeepVision: Benchmarking Deep Learning Architectures for Image Classification

## Overview

DeepVision is a comprehensive deep learning study focused on image classification across multiple benchmark datasets. The project investigates how different neural network architectures, optimization strategies, regularization techniques, and transfer learning approaches influence classification performance.

The study systematically compares Artificial Neural Networks (ANNs) and Convolutional Neural Networks (CNNs) while progressively introducing architectural improvements such as residual connections, global average pooling, depthwise separable convolutions, transfer learning, and advanced data augmentation techniques.

All models were implemented using PyTorch and evaluated using standard machine learning metrics including accuracy, precision, recall, F1-score, confusion matrices, and cross-validation.

---

## Objectives

- Compare the performance of ANN and CNN architectures on image classification tasks.
- Study the impact of transfer learning using pretrained models.
- Evaluate the effectiveness of residual learning and modern CNN design principles.
- Analyze the effect of regularization techniques and data augmentation methods.
- Understand how architectural choices influence model accuracy and generalization.

---

## Technologies Used

- Python
- PyTorch
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- Optuna

---

## Datasets

### 1. Fashion-MNIST

Fashion-MNIST is a benchmark dataset consisting of grayscale images of clothing items belonging to 10 categories.

Classes include:

- T-Shirt/Top
- Trouser
- Pullover
- Dress
- Coat
- Sandal
- Shirt
- Sneaker
- Bag
- Ankle Boot

---

### 2. CIFAR-10

CIFAR-10 is a widely used benchmark dataset containing RGB images belonging to 10 object categories.

Classes include:

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

---

### 3. Eye Disease Classification Dataset

A medical image classification dataset consisting of retinal eye images categorized into:

- Normal
- Cataract
- Glaucoma
- Retinal Disease

The dataset is used to evaluate deep learning models on real-world medical imaging tasks.

---

# Project Structure

```text
DeepVision-Image-Classification
│
├── notebooks
│   ├── fashion_MNIST_classification.ipynb
│   ├── cifar-10-classification.ipynb
│   └── eye-disease-classification.ipynb
│
├── report
│   └── DL_Project_Report.pdf
│
├── requirements.txt
│
└── README.md
```

---

# Models Implemented

## Fashion-MNIST

### ANN

A fully connected neural network with:

- Batch Normalization
- Dropout Regularization
- Hyperparameter Optimization using Optuna

### VGG16 Transfer Learning

A pretrained VGG16 model was used as a feature extractor with a custom classification head.

Features:

- Transfer Learning
- Frozen Convolutional Layers
- Fine-tuned Classifier Head

---

## CIFAR-10

### Baseline ANN

Traditional feed-forward neural network used as a baseline.

### Improved ANN

Enhancements include:

- Increased depth
- Increased width
- Improved dropout scheduling

### Baseline CNN

Convolutional neural network with:

- Convolution Layers
- Batch Normalization
- Max Pooling
- Spatial Dropout

### Deep CNN with Global Average Pooling (GAP)

Introduced:

- Deeper architecture
- Reduced parameter count
- Better generalization

### ResCNN

Residual CNN architecture inspired by ResNet.

Features:

- Skip Connections
- Improved Gradient Flow
- Reduced Vanishing Gradient Problem

### EfficientCNN

Depthwise Separable CNN inspired by MobileNet.

Features:

- Reduced Parameters
- Computational Efficiency
- Lightweight Architecture

### ResCNN with Mixup Augmentation

Combines:

- Residual Learning
- Mixup Data Augmentation

to improve robustness and generalization.

---

## Eye Disease Classification

### ANN Models

- Baseline ANN
- ANN with Regularization
- ANN with Early Stopping
- ANN with SGD Optimizer

### CNN Models

- Baseline CNN
- CNN with Batch Normalization
- CNN with Dropout
- CNN with Global Average Pooling
- CNN with Residual Connections

---

# Key Deep Learning Concepts Explored

This project explores several important deep learning concepts:

- Artificial Neural Networks (ANN)
- Convolutional Neural Networks (CNN)
- Transfer Learning
- Residual Learning
- Skip Connections
- Hyperparameter Optimization
- Batch Normalization
- Dropout Regularization
- Global Average Pooling (GAP)
- Mixup Data Augmentation
- K-Fold Cross Validation
- Confusion Matrix Analysis
- Model Generalization
- Medical Image Classification

---

# Evaluation Metrics

The following metrics were used to evaluate model performance:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Cross Validation Accuracy

These metrics provide a comprehensive assessment of both classification performance and model generalization.

---

# Key Findings

- CNN architectures consistently outperform ANN architectures for image classification tasks.
- Transfer Learning significantly improves performance on image datasets.
- Residual Connections improve gradient flow and enable deeper architectures.
- Global Average Pooling reduces parameter count while improving generalization.
- Mixup augmentation improves robustness and prevents model overconfidence.
- CNN-based approaches are more effective for medical image classification due to their ability to learn spatial and hierarchical features.

---

# Learning Outcomes

Through this project, I gained practical experience with:

- Building deep learning models using PyTorch
- Training and evaluating CNN architectures
- Transfer Learning using pretrained models
- Hyperparameter optimization using Optuna
- Image preprocessing and augmentation
- Medical image classification
- Model evaluation and performance analysis
- Deep learning experimentation and benchmarking

---

# Running the Project

## Clone Repository

```bash
git clone https://github.com/your-username/DeepVision-Image-Classification.git
```

## Install Dependencies

```bash
pip install -r requirements.txt
```

## Launch Jupyter Notebook

```bash
jupyter notebook
```

Open any notebook from the `notebooks` directory and execute the cells sequentially.

---

# Future Improvements

Potential future enhancements include:

- Vision Transformers (ViT)
- EfficientNet Architectures
- Self-Supervised Learning
- Explainable AI (Grad-CAM)
- Advanced Medical Imaging Models
- Model Deployment using Streamlit or Flask

---


