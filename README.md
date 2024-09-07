
# Semiconductor Manufacturing Yield Prediction (Utilising Feature Engineering)

## Problem Statement

In modern semiconductor manufacturing, hundreds of signals are collected from various sensors and measurement points. However, not all signals are equally valuable, and many of them contain noise or irrelevant data. Engineers typically work with more signals than are needed for specific tasks, making it crucial to identify the most relevant signals.

In this project, the goal is to develop a classifier that predicts whether a production entity will pass or fail based on available signal data. The project also involves determining whether all features (signals) are necessary or if a reduced set of signals can yield accurate predictions.

## Objectives

1. **Data Exploration and Cleansing**:
   - Load the provided dataset.
   - Handle missing values.
   - Drop irrelevant or redundant attributes based on functional knowledge and logical reasoning.
   - Modify the dataset as necessary to enhance feature relevance.

2. **Data Analysis and Visualization**:
   - Perform statistical analysis to understand the underlying structure of the data.
   - Conduct univariate, bivariate, and multivariate analysis to identify key patterns and relationships.
   - Provide detailed comments on all analyses conducted.

3. **Data Preprocessing**:
   - Segregate predictor attributes (features) and target attributes (Pass/Fail).
   - Check for imbalanced target classes and correct them if necessary.
   - Split the data into training and testing sets, ensuring that both sets are statistically similar to the original dataset.
   - Standardize the data if required to ensure consistency across features.

4. **Model Building and Evaluation**:
   - Choose and train a supervised machine learning model on the dataset.
   - Use cross-validation techniques to ensure the model generalizes well.
   - Apply hyper-parameter tuning to maximize model accuracy.
   - Explore additional techniques such as dimensionality reduction, feature removal, normalization, and target balancing to improve model performance.
   - Compare the performance of multiple models and select the best performing one.
   - Save the selected model for future use using model pickling.
   - Predict the yield type using future data and display the results.

5. **Conclusion and Recommendations**:
   - Analyze the results of the model, including its predictions and accuracy.
   - Discuss any potential improvements or next steps based on the model's performance.

## Dataset Overview

- **File Name**: `sensor-data.csv`
- **Shape**: 1567 samples and 591 features
- **Target Variable**: `Yield Type`, where:
  - `-1` indicates a pass.
  - `1` indicates a fail.

The dataset consists of measurements from various sensors, where each row represents a production entity, and each column represents a signal (feature) recorded at a specific test point. The goal is to predict whether a production entity will pass or fail based on the sensor signals.
