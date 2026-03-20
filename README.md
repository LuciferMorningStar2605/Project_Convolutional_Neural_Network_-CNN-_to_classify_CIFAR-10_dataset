# CIFAR-10 CNN Classifier

Notebook-based image classification project built on the CIFAR-10 dataset using a custom convolutional neural network in TensorFlow/Keras.

## Overview
This project walks through the standard deep learning workflow for CIFAR-10:
data preprocessing, normalization, label encoding, visual inspection, CNN training, and evaluation through test accuracy and a confusion matrix.

## Tech Stack
- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn

## Workflow
1. Load the CIFAR-10 dataset from `tf.keras.datasets`
2. Check for missing values and inspect class distribution
3. Normalize image pixels and reshape tensors for training
4. One-hot encode the labels
5. Train a CNN with stacked convolution, pooling, batch normalization, and dropout layers
6. Evaluate on the test split and visualize prediction quality with a confusion matrix

## Model Notes
- Loss: `categorical_crossentropy`
- Optimizer: `Adam`
- Regularization: dropout in intermediate and dense layers
- Evaluation artifact: confusion matrix on the test set

## Result
The saved notebook output shows test accuracy reaching roughly `75%` on CIFAR-10.

## Files
```text
Project_Convolutional_Neural_Network_-CNN-_to_classify_CIFAR-10_dataset/
├── Convolutional_Neural_ Network_to_classify_CIFAR-10.ipynb
└── README.md
```

## Run Locally
```bash
pip install tensorflow keras numpy pandas matplotlib seaborn
jupyter notebook "Convolutional_Neural_ Network_to_classify_CIFAR-10.ipynb"
```

## Learning Focus
- CNN design for small color images
- Image normalization and label encoding
- Overfitting control with dropout
- Interpreting confusion matrices for multi-class classification
