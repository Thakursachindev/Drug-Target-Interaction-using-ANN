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
![model_architecture](https://github.com/user-attachments/assets/6e8d475b-83b3-4254-9729-87719c0b1357)


## Hyperparameter Tuning
The model's hyperparameters are tuned using Hyperband:

units_input: Number of units in the input layer
number_of_layers: Number of hidden layers
learning_rate: Learning rate for optimization

![IMAGE 1](https://github.com/user-attachments/assets/22f9f08b-c28f-463a-b981-0d43b7880bf1)

## Training and Evaluation
The model is trained with 80% of the data, and 20% is held out for testing.
Metrics:
Accuracy: Model's accuracy on test data
Mean Squared Error (MSE): Prediction error on test data

![hyperband_trials-_1_](https://github.com/user-attachments/assets/397a7d3c-f786-4519-a4dd-3700aafc1578)


## Results and Visualizations
Best Model Performance:
Test Accuracy: Displayed in the notebook output
MSE: Displayed in the notebook output
Visualizations:
Model architecture
Validation accuracy over learning rates and layers
Graph representation of model layers

![IMAGE 2](https://github.com/user-attachments/assets/408df562-df48-48c0-8a2b-1701a0161fe3)
![IMAGE 3](https://github.com/user-attachments/assets/b049b7b3-945c-4290-a4b2-243a9781dd3c)
![IMAGE 5](https://github.com/user-attachments/assets/cc9790f1-0436-40ab-9e50-1a92e730493a)
![IMAGE 6](https://github.com/user-attachments/assets/400b9910-8217-4c51-a1df-72d9d3ff66a1)
![last image](https://github.com/user-attachments/assets/81c19aaf-fb17-4b09-9069-3d80c6e26a97)
