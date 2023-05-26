# Credit-Risk-Classification

This repository contains code for analyzing lending data and building a logistic regression model to predict loan status. The steps involved in the analysis and model building are described below.

# Importing the Modules

In this section, necessary modules such as numpy, pandas, and sklearn are imported. The pathlib module is used to handle file paths, and specific functions such as balanced_accuracy_score, confusion_matrix, and classification_report are imported from sklearn.metrics.

# Splitting the Data into Training and Testing Sets

In this section, the lending data is loaded from the 'lending_data.csv' file into a Pandas DataFrame. The data is split into labels (y) and features (X). The balance of the labels is checked using the value_counts function. The data is then split into training and testing datasets using the train_test_split function from sklearn.model_selection.

# Creating a Logistic Regression Model with the Original Data

In this section, a logistic regression model is fitted using the training data (X_train and y_train). The model is instantiated with a random_state parameter of 1. Predictions are made on the testing data (X_test) using the fitted model. The model's performance is evaluated by calculating the accuracy score, generating a confusion matrix, and printing the classification report.

# Predicting with a Logistic Regression Model Using Resampled Training Data

In this section, the data is resampled using the RandomOverSampler module from the imbalanced-learn library to address the imbalanced class distribution. The labels are oversampled to have an equal number of data points. Another logistic regression model is fitted using the resampled training data. Predictions are made on the testing data using the fitted model. The model's performance is evaluated by calculating the accuracy score, generating a confusion matrix, and printing the classification report.

# Summary
The logistic regression model is evaluated using the original data and then with resampled training data to address class imbalance. The performance of both models is assessed based on accuracy, precision, and other classification metrics. The results and findings are provided in the code comments.

Please refer to the code for more details on the implementation and analysis steps.
