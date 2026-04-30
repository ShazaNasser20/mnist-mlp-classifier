# Neural Networks Project - MLP for MNIST Classification

## Project Overview
This project implements a Multilayer Perceptron (MLP) model using TensorFlow/Keras to classify handwritten digits from the MNIST dataset.  
The goal is to build, train, and evaluate neural networks and compare different architectures and hyperparameters.

---

## Dataset
- Dataset: MNIST Handwritten Digits
- Source: Built-in dataset from TensorFlow/Keras
- Description:
  - 60,000 training images
  - 10,000 testing images
  - Image size: 28x28 pixels
  - Classes: 10 digits (0–9)

---

## Model Architecture

### Model 1 (Baseline)
- Input Layer: Flatten (28x28 → 784)
- Hidden Layer: 128 neurons (ReLU)
- Output Layer: 10 neurons (Softmax)

### Model 2 (Improved)
- Input Layer: Flatten (28x28 → 784)
- Hidden Layer 1: 256 neurons (ReLU)
- Hidden Layer 2: 128 neurons (ReLU)
- Output Layer: 10 neurons (Softmax)

---

## Training Details
- Optimizer: Adam
- Loss Function: Categorical Crossentropy
- Batch Size: 128
- Epochs: 10
- Validation Split: 20%

---

## Evaluation Metrics
The models were evaluated using:
- Accuracy
- Loss

---

## Results

| Model    | Architecture          | Accuracy | Loss   |
|----------|----------------------|----------|--------|
| Model 1  | 128 neurons          | 97.25%   | 0.0848 |
| Model 2  | 256 + 128 neurons    | 97.84%   | 0.0743 |

Sample Results:
Model 2 achieved the best performance with higher accuracy and lower loss.

---

## Visualizations
The project includes:
- Training vs Validation Loss curves
- Training vs Validation Accuracy curves

---

## Experiments
Two experiments were conducted by modifying:
- Number of neurons in hidden layers
- Number of hidden layers
- Learning rate

Model 2 showed better performance compared to Model 1.

---

## How to Run the Project

Install dependencies:
pip install tensorflow numpy matplotlib

Run the notebook:
Open the Jupyter Notebook or Google Colab file and execute all cells sequentially.

---

## Author
Shaza Abdulnaser Sayed  
Faculty of Artificial Intelligence and Data Management  

---

## Notes
This project is part of the Neural Networks course requirements.  
It demonstrates the implementation and evaluation of an MLP model for image classification.
