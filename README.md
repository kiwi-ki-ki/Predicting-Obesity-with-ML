# Predicting-Obesity-with-ML

## Overview 
The purpose of this project was to accurately predict obesity based on biological, lifestyle, and personal demographic features. The script implemented four separate models, including a baseline random classifier, a multinomial logistic regression (MLR), a Gaussian Naive Bayes model, and a multi-layer perceptron neural network (MLP). The data was sourced from the UCI Machine Learning Repository – “Estimation of Obesity Levels Based on Eating Habits and Physical Condition”.

## Method 
The random classifier was built using Scikit-Learn's DummyClassifier and evaluated using accuracy and a confusion matrix.

The MLR model was built using Scikit-Learn's LogisticRegression with the lbfgs solver, selected for its ability to handle high-dimensional data. This model was also evaluated using accuracy and a confusion matrix.

The Naive Bayes model was developed using Scikit-Learn's GaussianNB and was similarly evaluated with accuracy and a confusion matrix.

The MLP was constructed using a sequential neural network from Keras (TensorFlow) with two hidden layers, each using the ReLU activation function. The output layer used the softmax activation function, and the model was compiled with the Adam optimizer and a learning rate of 0.001. This model was evaluated by plotting the learning curves for both accuracy and loss.

To verify that overfitting was not present, each model was also tested on shuffled target (y) data.

## Results
The accuracy for each model was calculated as follows:
• Random Classifier Accuracy: 0.1316
• Multinomial Logistic Regression Accuracy: 0.9785
• Naive Bayes Accuracy: 0.9928
• MLP Test Accuracy: 0.9880

## Note 
This project was conducted as a practice exercise for applying machine learning models to real-world data and is not intended for legitimate medical analysis. Limitations of this project include the small number of cases in the data and the use of accuracy as the sole evaluation metric.
