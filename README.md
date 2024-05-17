Neural Network SMS Text Classifier Project
Project Overview

This project involves creating a machine learning model to classify SMS messages as either "ham" (normal messages) or "spam" (unwanted advertisements). The classifier is built using a neural network and is trained on the SMS Spam Collection dataset. The primary goal is to accurately identify and distinguish between legitimate messages and spam messages.

Key Steps in the Project
Data Loading and Exploration:

The SMS Spam Collection dataset is loaded, which contains SMS messages labeled as "ham" or "spam".
Data Preprocessing:

The text data is cleaned and preprocessed. Labels are encoded into binary format where "ham" is 0 and "spam" is 1.
The data is split into training and testing sets to evaluate the model's performance.
Text Tokenization and Padding:

Tokenization converts the text messages into sequences of integers.
Padding ensures all sequences have the same length, which is necessary for training the neural network.
Model Building:

A neural network model is created using Keras, consisting of an embedding layer, an LSTM (Long Short-Term Memory) layer, and a dense output layer with a sigmoid activation function.
Model Training:

The model is trained on the training data using the Adam optimizer and binary cross-entropy loss function.
Model Evaluation:

The model's performance is evaluated on the test data to measure its accuracy.
Prediction Function:

A function predict_message is implemented to classify new messages. It returns the probability of the message being spam and the corresponding label ("spam" or "ham").
Example Usage
The project includes example usage of the predict_message function to demonstrate how the model classifies new SMS messages.

python
Copy code
print(predict_message("Congratulations! You've won a free ticket to the Bahamas. Call now!"))
print(predict_message("Hey, are we still meeting for coffee at 4pm?"))
Technologies and Libraries Used
Python: The programming language used for this project.
Pandas: For data manipulation and analysis.
NumPy: For numerical computations.
Scikit-learn: For data preprocessing and model evaluation.
Keras with TensorFlow backend: For building and training the neural network model.
Objective
The objective of this project is to create a reliable SMS spam detection system using neural networks, providing accurate predictions and helping to filter out unwanted spam messages. This project serves as a practical application of machine learning and natural language processing techniques.
