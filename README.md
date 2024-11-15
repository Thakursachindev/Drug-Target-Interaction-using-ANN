# Drug Target Interaction Using Artificial Neural Network (Feed Forwarded Neural Network (FNN) )

## Table of Contents
- Installation
- Data
- Model Architecture
- Hyper Parameter Tuning
- Training Evualation
- Results and Visualizations

## Installation
pip install keras-tuner pandas numpy scikit-learn tensorflow matplotlib networkx graphviz

## Data
The model is trained and tested on the synthetic_drug_target_interaction.csv dataset:

Features: Drug and target interaction features
Target: Interaction outcome.

## Model Architecture
The model is a feedforward neural network with tunable layers. Key components:

Input layer with varying units (32 to 512)
Hidden layers with ReLU activation
Output layer for binary classification

## Hyperparameter Tuning
The model's hyperparameters are tuned using Hyperband:

units_input: Number of units in the input layer
number_of_layers: Number of hidden layers
learning_rate: Learning rate for optimization

## Training and Evaluation
The model is trained with 80% of the data, and 20% is held out for testing.
Metrics:
Accuracy: Model's accuracy on test data
Mean Squared Error (MSE): Prediction error on test data

## Results and Visualizations
Best Model Performance:
Test Accuracy: Displayed in the notebook output
MSE: Displayed in the notebook output
Visualizations:
Model architecture
Validation accuracy over learning rates and layers
Graph representation of model layers

