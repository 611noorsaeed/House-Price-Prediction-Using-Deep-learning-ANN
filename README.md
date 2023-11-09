# House-Price-Prediction-Using-Deep-learning-ANN

Table of Contents


Introduction
Data Preprocessing
Neural Network Architecture
Model Training
Model Evaluation
Web Application using Flask
Documentation for Flask App
1. Introduction

The House Price Prediction System is designed to predict house prices based on various features like location, room details, and other amenities. The system utilizes a neural network model implemented using the Keras framework. Additionally, a Flask web application has been developed to provide an intuitive interface for users to input data and receive price predictions.


2. Data Preprocessing
Data Scaling: Features are scaled using the Min-Max Scaler from scikit-learn to ensure consistent input to the neural network.
Data Splitting: The dataset is split into training and testing sets to evaluate the model's performance accurately.

3. Neural Network Architecture
The neural network architecture consists of an input layer, two hidden layers with dropout for regularization, and an output layer for regression.

Input Layer: 1000 neurons, ReLU activation
Dropout Layer: 20% dropout rate
Hidden Layer 1: 500 neurons, ReLU activation
Dropout Layer: 20% dropout rate
Hidden Layer 2: 250 neurons, ReLU activation
Output Layer: 1 neuron, linear activation for regression
4. Model Training

The model is compiled using the RMSprop optimizer and Mean Squared Error loss function. Early stopping is implemented with a patience of 50 epochs to prevent overfitting. The training is performed for 10 epochs with a batch size of 50.

5. Model Evaluation

The model is evaluated using various metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), Mean Squared Log Error (MSLE), and R-squared score on the testing dataset.

6. Web Application using Flask

A Flask web application has been created to provide a user-friendly interface for predicting house prices. The application loads the pre-trained neural network model and scaler. Users can input information such as longitude, latitude, house age, and other details to get a predicted house price.
