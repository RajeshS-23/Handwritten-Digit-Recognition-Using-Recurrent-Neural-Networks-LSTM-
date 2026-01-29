# Handwritten Digit Recognition Using Recurrent Neural Networks (LSTM)

This project implements handwritten digit classification on the MNIST dataset
using a Recurrent Neural Network (RNN) based on Long Short-Term Memory (LSTM).

Although MNIST is an image dataset, it is converted into sequential data by
treating each image as a sequence of rows, enabling the use of LSTM networks.

---

## Dataset

- Dataset Name: MNIST
- Image Size: 28 × 28 pixels
- Color Format: Grayscale
- Number of Classes: 10 (Digits 0–9)
- Training Samples: 60,000
- Testing Samples: 10,000

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib

---

## Model Architecture

- Input layer with shape (28, 28)
- LSTM layer with 128 units (returns sequences)
- LSTM layer with 64 units
- Dropout layer to reduce overfitting
- Dense output layer with Softmax activation

---

## Loss Function and Optimizer

- Loss Function: Sparse Categorical Crossentropy
- Optimizer: Adam
- Evaluation Metric: Accuracy

---

## Training Details

- Epochs: 10
- Data Normalization: Pixel values scaled to range [0, 1]
- Validation: Test dataset used for validation

---

## Results

The LSTM-based RNN successfully learns sequential patterns from MNIST images.
While CNNs generally perform better on image data, this project demonstrates
how RNNs can be adapted for image classification by reshaping images into sequences.

---

## How to Run the Project

1. Install required libraries:
   ```bash
   pip install tensorflow matplotlib numpy
