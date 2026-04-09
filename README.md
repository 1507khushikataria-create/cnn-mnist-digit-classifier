# cnn-mnist-digit-classifier
This project implements a Convolutional Neural Network (CNN) using PyTorch to classify handwritten digits from the MNIST dataset. It covers data preprocessing, model training, and performance evaluation using accuracy and loss metrics. The implementation demonstrates core deep learning concept and supports GPU acceleration with CUDA when available.
# MNIST CNN Digit Classifier

## Project Overview

This project implements a Convolutional Neural Network (CNN) using PyTorch to classify handwritten digits from the MNIST dataset. The model is trained to recognize digits from 0 to 9 using labeled image data.

The goal of this project is to demonstrate the fundamental concepts of deep learning, including convolutional layers, activation functions, pooling, model training, and evaluation. The implementation covers the complete machine learning workflow from data loading to model performance evaluation.

This project is part of a machine learning portfolio showcasing practical implementation of neural networks using Python and PyTorch.

---

## Dataset

The MNIST dataset is a standard benchmark dataset widely used in machine learning and deep learning.

Dataset details:

* Number of classes: 10 (digits 0–9)
* Image size: 28 × 28 pixels
* Training samples: 60,000
* Test samples: 10,000
* Image type: Grayscale

The dataset is automatically downloaded using the Torchvision library when the training script is executed.

---

## Model Architecture

The Convolutional Neural Network (CNN) used in this project consists of the following layers:

1. Convolutional Layer

   * 32 filters
   * Kernel size: 3 × 3
   * Activation function: ReLU

2. Max Pooling Layer

   * Pool size: 2 × 2

3. Convolutional Layer

   * 64 filters
   * Kernel size: 3 × 3
   * Activation function: ReLU

4. Max Pooling Layer

5. Fully Connected Layer

   * 128 neurons
   * Activation function: ReLU

6. Output Layer

   * 10 neurons representing digits 0–9

---

## Technologies Used

* Python
* PyTorch
* Torchvision
* NumPy
* Matplotlib

---

## How the Model Works

The CNN processes input images through convolutional layers that extract important visual features such as edges, curves, and shapes.

Pooling layers reduce the size of feature maps while preserving essential information.

Fully connected layers combine extracted features to make predictions about which digit is present in the image.

---

## Training Process

The model training process includes the following steps:

1. Load the MNIST dataset
2. Normalize image pixel values
3. Initialize the CNN model
4. Define the loss function
5. Define the optimizer
6. Train the model for multiple epochs
7. Calculate training accuracy and loss
8. Save the trained model

Loss Function used:

CrossEntropyLoss

Optimizer used:

Adam optimizer

---

## Evaluation Metrics

The model performance is evaluated using:

Accuracy
Loss

Accuracy measures how many predictions are correct.
Loss measures how far predicted values are from the actual values.

---

## Results

Typical results for this model:

Training Accuracy: approximately 99%
Test Accuracy: approximately 98%

The loss decreases steadily during training, indicating that the model is learning effectively.

---

## Installation

Step 1: Clone the repository

git clone https://github.com/your-username/mnist-cnn-pytorch.git

Step 2: Navigate to the project directory

cd mnist-cnn-pytorch

Step 3: Install dependencies

pip install -r requirements.txt

---

## How to Run the Project

Train the model:

python train.py

Test the model:

python test.py

---

## GPU Support

The program automatically checks whether a GPU is available.

If a GPU is available:

Using device: cuda

Otherwise:

Using device: cpu

Using a GPU significantly improves training speed and performance.

---

## Future Improvements

Possible future enhancements include:

* Implementing deeper CNN architectures
* Adding data augmentation techniques
* Hyperparameter tuning
* Deploying the model using FastAPI
* Adding real-time prediction functionality
* Visualizing results using confusion matrix

---

## Learning Outcomes

This project demonstrates:

* Understanding of Convolutional Neural Networks (CNN)
* Training deep learning models using PyTorch
* Data preprocessing and normalization
* Model evaluation and performance tracking
* Working with GPU acceleration
* Building structured machine learning projects

---

## Author

Khushi Kataria
Machine Learning / AI Portfolio Project
