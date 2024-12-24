# Cancer Prediction
This project aims to predict the type of cancer for a patient using machine learning.

## Project Overview
This project implements a machine learning pipeline to classify breast cancer as Benign or Malignant using the k-Nearest Neighbors (k-NN) algorithm. The dataset is preprocessed to handle categorical data, scaled for consistency, and split into training and testing sets to evaluate model performance. The goal is to provide a simple, scalable approach to cancer diagnosis prediction, demonstrating the use of basic ML techniques with Python and scikit-learn.

## Dataset
This project utilizes the Cancer dataset, which includes patient(s)'s cancer related intel. This dataset contains 569 rows and 33 columns.

## Execution Plan

The methodology outlines the step-by-step process followed to design, train, evaluate, and deploy the machine learning model for predicting breast cancer as either Benign or Malignant. The pipeline ensures data integrity, scalability, and efficient learning using the k-Nearest Neighbors (k-NN) algorithm.

**1. Understanding the Problem:** The objective is to classify breast cancer tumors into Benign (non-cancerous) or Malignant (cancerous) based on diagnostic features, aiding early diagnosis and treatment.

**2. Dataset Preparation:** The dataset is loaded from a CSV file and includes diagnostic features such as radius_mean, texture_mean, perimeter_mean, and area_worst, along with a target variable (diagnosis) indicating tumor type.

**3. Preprocessing:** The diagnosis column is encoded into numerical values (0 for benign, 1 for malignant), and the data is checked for missing values to ensure integrity.

**4. Feature Scaling:** The feature values are normalized using MinMaxScaler to ensure uniformity, as k-NN relies on distance metrics.

**5. Data Splitting:** The dataset is split into a training set (70%) and a testing set (30%) using train_test_split to evaluate the model's performance on unseen data.

**6. Model Training:** The k-Nearest Neighbors (k-NN) algorithm is selected, and the model is trained with n_neighbors=8 on the normalized training dataset.

**7. Model Evaluation:** The model is tested on the testing dataset, and its accuracy is calculated to assess how well it generalizes to unseen data.

**8. Prediction Pipeline:** New sample data is normalized using the scaler, and the trained k-NN model predicts whether the tumor is Benign or Malignant.

## Results

The k-Nearest Neighbors (k-NN) model achieved an accuracy of approximately X%, successfully classifying tumors as Benign or Malignant. A sample input ([0, 0, 0.299, 0.33]) was correctly predicted, demonstrating the model's real-world applicability.

