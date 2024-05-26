# SSDI Benefits Fraud Detection Project

This project aims to identify potential Social Security Disability Insurance (SSDI) benefits fraud by comparing the Social Security Numbers (SSNs) of individuals earning above a certain threshold with those receiving SSDI benefits. By leveraging data visualization and machine learning techniques, we can efficiently flag cases for further investigation.

## Overview

### Objective

The objective of this project is to develop a system that can identify potential fraud cases by:
1. Comparing SSNs of individuals earning above $1,550 per month with those receiving SSDI benefits.
2. Flagging overlapping SSNs for further investigation.

### Methodology

The project is divided into several key steps:
1. **Data Preparation**: Collect and preprocess the data.
2. **Feature Engineering**: Create meaningful features from the raw data.
3. **Model Selection**: Choose an appropriate machine learning model for classification.
4. **Training and Evaluation**: Train the model and evaluate its performance.
5. **Prediction and Visualization**: Use the trained model to predict potential fraud cases and visualize the results.

## Data Preparation

We start by preparing the data, which includes SSNs, earnings, and SSDI status. The data is then split into training and testing sets. Here, we also standardize the features to improve the model's performance.

## Data Visualization  

To better understand our data, we use visualizations. Here are some key visualizations we use in this project:  
1. **Distribution of Earnings: A histogram to show the distribution of earnings.
2. **Confusion Matrix: A heatmap to visualize the model's performance.
3. **ROC Curve: To evaluate the model's trade-off between true positive and false positive rates.

## Model Training and Evaluation  

We use a Logistic Regression model to classify whether individuals are receiving SSDI benefits based on their earnings and other features. The model is trained and evaluated on our dataset.

## Prediction and Visualization  

Finally, we use the trained model to make predictions on new data and visualize the results to understand which SSNs are flagged for further investigation.

---

## Python Code Explanation  

Data Preparation:

The data is loaded into a DataFrame, and a new feature Above_Threshold is created to indicate if earnings exceed $1,550 per month.
Visualization:

A histogram is plotted to visualize the distribution of earnings in the dataset.
Model Training:

The dataset is split into training and testing sets.
Features are standardized using StandardScaler.
A logistic regression model is trained on the training set.
Model Evaluation:

Predictions are made on the test set.
The model's performance is evaluated using accuracy, precision, recall, and F1 score.
A confusion matrix and ROC curve are plotted for better visualization of the model's performance.
Prediction:

New data is processed, and predictions are made using the trained model.
Results are visualized using a bar plot.

