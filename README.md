# Neural Networks Project - MLP for MNIST Classification

## Project Overview
This project implements a Multilayer Perceptron (MLP) model using TensorFlow/Keras to classify handwritten digits from the MNIST dataset.  
The goal is to build, train, and evaluate a neural network and compare different architectures and hyperparameters.

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

---

## Visualizations
The following plots are included in the project:
- Training vs Validation Loss
- Training vs Validation Accuracy

---

## Experiments
Two experiments were conducted by modifying:
- Number of neurons in hidden layers
- Model depth (number of hidden layers)
- Learning rate (in Model 2)

Model 2 showed improved performance compared to the baseline model.

---

## How to Run the Project

### Install dependencies
pip install tensorflow numpy matplotlib

### Run the notebook
Open the Jupyter Notebook or Google Colab file and run all cells sequentially.

---

## Project Structure

MNIST-MLP-Project/
│
├── notebook.ipynb
├── README.md
├── results/
│   └── plots/
└── data/ (optional)

---

## Author
Shaza Abdulnaser Sayed  
Faculty of Artificial Intelligence and Data Management  

---

## Notes
- This project is implemented as part of the Neural Networks course requirements.
- The MLP model is used for educational purposes to understand deep learning fundamentals.
