# Iris Dataset Classification Project

## Project Overview

This project involves building and evaluating various machine learning models to classify the species of iris flowers based on their physical attributes: sepal length, sepal width, petal length, and petal width. The dataset used in this project is the famous Iris dataset.

## Objectives

1. Load and preprocess the dataset.
2. Handle missing values.
3. Identify and handle outliers.
4. Split the dataset into training and testing sets.
5. Train and evaluate multiple machine learning models.
6. Compare the models based on accuracy, training time, and prediction time.
7. Select the best model based on the evaluation criteria.

## Dataset

The Iris dataset contains 150 samples of iris flowers, with each sample having four features:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

The target variable is the species of the iris flower, which can be one of three classes:
- Setosa
- Versicolor
- Virginica

## Outlier Detection and Handling

Outliers can significantly affect the performance of machine learning models. In this project, outliers were detected using z-scores calculated within each species group. Z-scores measure the number of standard deviations a data point is from the mean. Data points with z-scores greater than 3 or less than -3 were considered outliers and removed from the dataset to improve the model's performance and robustness.


## Models Evaluated

The following machine learning models were evaluated:
- K-Nearest Neighbors (KNN)
- Random Forest
- Logistic Regression
- Support Vector Classifier (SVC)

## Evaluation Criteria

Each model was evaluated based on:
- Accuracy: The proportion of correctly classified samples.
- Training Time: The time taken to train the model.
- Prediction Time: The time taken to make predictions on the test set.

## Results

The evaluation results for each model are summarized in the table below:

| Model               | Accuracy | Training Time (s) | Prediction Time (s) |
|---------------------|----------|-------------------|----------------------|
| K-Nearest Neighbors | 1.00     | 0.002             | 0.002                |
| Random Forest       | 1.00     | 0.06              | 0.005                |
| Logistic Regression | 1.00     | 0.02              | 0.001                |
| SVC                 | 1.00     | 0.002             | 0.002                |

## Model Selection

The primary criterion for model selection was accuracy, as it directly measures the proportion of correctly classified samples. For this dataset, accuracy is a suitable metric because:
- The dataset is balanced, with an equal number of samples for each class.
- The primary goal is to correctly classify the species of iris flowers.

In case of a tie in accuracy, the model with the lesser training time was chosen. Based on the evaluation, the **k-Nearest Neighbors** model had the highest accuracy (1.00) and the lowest computing time. Therefore, the k-Nearest Neighbors is selected as the best model for this classification task.

## Conclusion

In this project, we successfully built and evaluated multiple machine learning models to classify the species of iris flowers. The k-Nearest Neighbors model was selected as the best model based on its accuracy. 
