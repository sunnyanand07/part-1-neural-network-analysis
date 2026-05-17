Customer Churn Prediction using Neural Networks
Overview

This project demonstrates how to build a Neural Network model for Customer Churn Prediction using Python, TensorFlow/Keras, and Machine Learning preprocessing techniques.

The notebook covers the complete workflow from data preprocessing to model training, evaluation, and hyperparameter experimentation.

The main objective of this assignment is to predict whether a customer will churn based on different customer-related features.

Technologies and Libraries Used
Python
TensorFlow / Keras
NumPy
Pandas
Matplotlib
Seaborn
Scikit-learn
Project Workflow
1. Importing Libraries

The notebook begins by importing all required libraries for:

Data handling
Data visualization
Data preprocessing
Neural network model building
Performance evaluation
2. Dataset Loading

The dataset is loaded into a Pandas DataFrame.

Basic dataset inspection is performed using:

Shape of dataset
Data types
Null value checking
Statistical summary
3. Exploratory Data Analysis (EDA)

Visualization techniques are used to understand the dataset.

Operations Performed:
Churn distribution visualization using Countplot
Feature analysis
Data understanding before preprocessing
4. Data Preprocessing

Several preprocessing techniques are applied before training the neural network.

Preprocessing Steps:
a) Removing Unnecessary Columns

The customer_id column is removed because it does not contribute to prediction.

b) Label Encoding

Categorical features are converted into numeric form using LabelEncoder.

Encoded columns include:

region
plan_type
contract_type
payment_method
c) Feature Scaling

StandardScaler is used to normalize the input features.

Feature scaling improves neural network performance and training stability.

5. Splitting Dataset

The dataset is divided into:

Training Data
Testing Data

using train_test_split().

Neural Network Model
6. Model Architecture

A Sequential Neural Network model is created using Keras.

Layers Used:
Layer	Details
Input Layer	Dense layer with 16 neurons and ReLU activation
Hidden Layer	Dense layer with 8 neurons and ReLU activation
Output Layer	Dense layer with 1 neuron and Sigmoid activation
Activation Functions:
ReLU for hidden layers
Sigmoid for binary classification
7. Model Compilation

The model is compiled using:

Optimizer: Adam
Loss Function: Binary Crossentropy
Metric: Accuracy
8. Model Training

The model is trained using:

Epochs: 20
Batch Size: 32
Validation Split: 0.2

Training history is stored for visualization.

Model Evaluation
9. Accuracy and Loss Graphs

Graphs are plotted for:

Training Accuracy
Validation Accuracy
Training Loss
Validation Loss

These graphs help in understanding:

Model learning performance
Overfitting or underfitting
Training stability
10. Testing the Model

The trained model is evaluated on test data.

Evaluation metrics include:

Test Loss
Test Accuracy
11. Predictions

Predictions are generated using the trained model.

The output probabilities are converted into binary values using a threshold of 0.5.

12. Confusion Matrix

A confusion matrix is generated using Seaborn heatmap.

It helps analyze:

Correct predictions
False positives
False negatives
13. Classification Report

The classification report includes:

Precision
Recall
F1-score
Accuracy

This provides detailed model performance analysis.

Hyperparameter Experimentation

An improved model is created with:

More neurons
Additional hidden layer capacity
Increased epochs
Updated Configuration:
Parameter	Value
Hidden Layer 1	32 neurons
Hidden Layer 2	16 neurons
Epochs	50
Optimizer	Adam
Learning Rate	0.001

This experimentation helps compare model performance and improve accuracy.

Results

The neural network model successfully learns patterns from the customer dataset and predicts customer churn with good performance.

The assignment demonstrates:

Data preprocessing
Neural network implementation
Model evaluation
Performance visualization
Hyperparameter tuning
Key Concepts Learned
Artificial Neural Networks (ANN)
Data preprocessing techniques
Feature scaling
Label encoding
Binary classification
Model training and evaluation
Confusion matrix interpretation
Hyperparameter tuning
Conclusion

This project provides practical experience in building a deep learning classification model using TensorFlow/Keras.

The notebook follows a complete machine learning workflow from raw dataset preprocessing to final prediction and evaluation.

The assignment also highlights the importance of:

Proper preprocessing
Model architecture selection
Training optimization
Performance evaluation