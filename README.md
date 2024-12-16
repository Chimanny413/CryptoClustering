# Credit Risk Classification

## Overview

This project focuses on predicting the creditworthiness of borrowers using a logistic regression model. The dataset contains historical lending activity data, where the goal is to classify loans as either **low-risk (healthy)** or **high-risk (default-prone)**. This classification helps financial institutions manage risk and make informed decisions.

## Objectives

-   **Analyze Loan Risk**: Identify patterns in the data to predict loan outcomes.

-   **Build a Logistic Regression Model**: Train a binary classification model to separate high-risk loans from low-risk loans.

-   **Evaluate Model Performance**: Assess the reliability and accuracy of the model using standard performance metrics.

## Methodology

### 1. Data Preprocessing

-   **Dataset Loading**: The *lending_data.csv* file was loaded into a Pandas DataFrame.

-   **Feature and Label Separation**:

    - The *loan_status* column was used as the target variable *(y)*, where 0 indicates a low-risk loan and 1 indicates a high-risk loan.

    - The remaining columns served as features *(X)*.

-   **Data Splitting**: Used Scikit-learn’s *train_test_split* function to divide the data into training and testing subsets to ensure unbiased model evaluation.

### 2. Logistic Regression Model

-   Model Training: Initialized and trained a logistic regression model on the training data *(X_train* and *y_train)*.

-   Prediction: Used the trained model to predict loan outcomes on the testing data *(X_test)*.

### 3. Model Evaluation

-   **Confusion Matrix**: Generated a confusion matrix to visualize classification results, including true positives, false positives, true negatives, and false negatives.

-   **Classification Report**: Calculated key metrics:

    - **Accuracy**: Overall correctness of the model.

    - **Precision**: Proportion of high-risk loans correctly identified.

    - **Recall**: Proportion of all actual high-risk loans that were detected.
