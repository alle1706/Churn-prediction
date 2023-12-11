# Churn-prediction
ANN tensorflow model built on bank costumers dataset

## Overview

This repository contains a churn prediction model implemented using Artificial Neural Networks (ANN) for predicting customer churn in a bank's customer dataset. The model is developed using Python and the TensorFlow library.

## Dataset

The model was trained on a dataset sourced from Kaggle, which you can find [here](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia).


## Data Preprocessing

The initial dataset is loaded from "Churn_Modelling.csv."
Irrelevant columns like 'CustomerId,' 'Surname,' 'RowNumber,' and 'Geography' are dropped.
Data types are checked to ensure proper encoding.
The 'Gender' column is encoded (Female: 1, Male: 0).
Selected columns ('CreditScore', 'Age', 'Tenure', 'Balance', 'NumOfProducts', 'EstimatedSalary') are scaled using Min-Max scaling.

## Training and architecture

- An ANN model is constructed using TensorFlow's Keras API.
The model architecture consists of an input layer with 26 neurons, a hidden layer with 15 neurons, and an output layer with 1 neuron using the sigmoid activation function.
- The model is compiled using the Adam optimizer and binary cross-entropy loss.
Training is performed for 100 epochs.

## Evaluation

The trained model is evaluated on the test set, resulting in an accuracy of approximately 85%.


## Future Work

Future improvements may include fine-tuning the model for enhanced accuracy.

## Technologies Used

- TensorFlow
- Python
- Keras
- Scikit-learn
