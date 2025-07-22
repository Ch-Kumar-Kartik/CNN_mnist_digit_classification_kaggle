# MNIST Digit Recognizer CNN

This repository contains implementation of a Convolutional Neural Network (CNN) for the MNIST Digit Recognizer competition on Kaggle. The project achieved a validation accuracy of 99.18% and a Kaggle public leaderboard score of 98.057%.

## Project Overview

Built this CNN to classify handwritten digits (0-9) from the MNIST dataset, a classic machine learning benchmark. The project includes data preprocessing, model training, visualization, Kaggle submission, and custom digit testing.

## Features

- **Data Preprocessing**: Normalizes and reshapes MNIST data into 28x28x1 tensors.
- **CNN Architecture**: Two blocks of `[Conv2D->relu]*2 -> MaxPool2D -> Dropout(0.25)` with 32/64 filters, followed by `Flatten -> Dense(256, relu) -> Dropout(0.5) -> Dense(10, softmax)`.
- **Training**: Utilizes TensorFlow/Keras with Adam optimizer, achieving 99.30% training and 99.18% validation accuracy over 5 epochs.
- **Visualization**: Plots training/validation accuracy and loss using Matplotlib.
- **Kaggle Submission**: Generates a submission.csv file with a score of 98.057%.
- **Custom Testing**: Allows drawing digits interactively to test model predictions. (won't work in kaggle)

## Installation

### Prerequisites
- Python 3.7+
- Required libraries: `tensorflow`, `keras`, `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `Pillow`

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/mnist-digit-recognizer-cnn.git
   cd mnist-digit-recognizer-cnn
