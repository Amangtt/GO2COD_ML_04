# GO2COD_ML_04
Iris Flower Classification with TensorFlow

This repository implements a machine learning model using TensorFlow's Keras API to classify Iris flower species based on their sepal and petal measurements.

Clone the repository:
git clone https://github.com/Amangtt/iris-classification.git

Install dependencies:
Navigate to the project directory and run:
pip install tensorflow pandas numpy sklearn matplotlib

Run the script
python iris_classification.py

Description

The script performs the following steps:

Data Loading and Preprocessing:

Reads the Iris flower dataset 
Separates features (x) and target labels (y).
Encodes target labels using a scikit-learn LabelEncoder.
Splits the data into training, validation (cv), and testing sets using train_test_split.

Model Definition:

Defines a sequential TensorFlow model with three dense layers:
Layer 1: Input layer with 64 neurons and ReLU activation.
Layer 2: Hidden layer with 128 neurons and ReLU activation.
Layer 3: Output layer with 3 neurons (one for each flower species) and linear activation.

Model Compilation:

Compiles the model using the following parameters:
Loss function: Sparse categorical cross-entropy (suitable for multi-class classification).
Optimizer: Adam optimizer with a learning rate of 0.001.
Metrics: Monitors training and validation accuracy.

Model Training:

Trains the model on the training data for 30 epochs.

Model Evaluation:

Evaluates the model's performance on both the training and validation sets using accuracy.
Prints the test accuracy for both sets.
Creates a confusion matrix to visualize the model's prediction distribution across classes.
Generates a classification report with detailed metrics (precision, recall, F1-score, support) for each class.

Visualization:

Plots the true labels and predicted labels for the training data to visually assess performance (optional).
