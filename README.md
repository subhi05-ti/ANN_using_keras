# ANN_using_keras
Customer Churn Prediction Using Neural Networks (Keras)
This project demonstrates how to predict customer churn using an Artificial Neural Network (ANN) built with TensorFlow/Keras. The dataset used is the popular Churn_Modelling.csv file, which contains information about customers of a bank, and the goal is to predict whether a customer will leave (churn) or not.

-> Dataset Overview
Source: Churn_Modelling.csv

Target Variable: Exited (1 = churned, 0 = retained)

Features Include:

Demographics: Geography, Gender, Age

Account Info: Balance, Tenure, NumOfProducts

Credit Score and Salary details

-> Workflow
Data Preprocessing

Loaded and cleaned the data

Encoded categorical features (Geography and Gender)

Dropped non-informative columns: RowNumber, CustomerId, Surname

Split into train and test sets

Scaled features using StandardScaler

Model Building

Used Keras Sequential API to build a neural network

-> Architecture:

Input Layer: 10 features

Hidden Layers: 2 layers with 16 neurons each and ReLU activation

Output Layer: 1 neuron with Sigmoid activation for binary classification

-> Training

Optimizer: Adam

Loss Function: Binary Crossentropy

Metrics: Accuracy

Trained for 10 epochs with validation_split=0.2

-> Evaluation

Evaluated the model using accuracy_score on the test set

Visualized loss and validation loss using matplotlib

-> Model Performance
Test Accuracy: ~Achieved from model evaluation
