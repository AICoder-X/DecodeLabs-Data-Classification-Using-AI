# DATA CLASSIFICATION USING AI

A simple yet functional **KNN-based classification model** built using Python and Scikit-learn. This project demonstrates how supervised machine learning can be used to classify flower species based on numerical features. The model trains on the Iris dataset, finds the optimal K using the Elbow Method, and evaluates performance using accuracy, F1 score, and a confusion matrix — making it a practical and educational intermediate-level project.

---

## 📌 Table of Contents

- [📖 Overview](#-overview)  
- [✨ Features](#-features)  
- [🛠️ Technologies Used](#️-technologies-used)  
- [🚀 Code](#-code)  
- [🔧 Future Enhancements](#-future-enhancements)  

---

## 📖 Overview

This project is a **command-line based AI classification system** that uses the **K-Nearest Neighbors (KNN)** algorithm to classify iris flowers into three species: Setosa, Versicolor, and Virginica. It takes four numerical measurements as input (sepal length, sepal width, petal length, petal width) and predicts the correct species.

It's an intermediate-level project to explore how supervised learning works and lays the foundation for more advanced concepts like neural networks and deep learning.

---

## ✨ Features

- Loads and explores the **Iris benchmark dataset**
- Applies **StandardScaler** for feature normalization
- Splits data into **80% training / 20% testing sets**
- Finds the **optimal K** automatically using the Elbow Method
- Trains a **KNN classifier** and makes predictions
- Evaluates model using:
  - Accuracy Score
  - Weighted F1 Score
  - Classification Report
  - Confusion Matrix
- Generates **3 visualizations**: Elbow Curve, Confusion Matrix Heatmap, Feature Scatter Plot
- Includes a **live prediction demo** on a new custom sample

---

## 🛠️ Technologies Used

- **Language**: Python 3.x
- **Libraries**:
  - numpy — numerical operations
  - pandas — data loading and exploration
  - matplotlib & seaborn — visualizations
  - scikit-learn — ML pipeline (scaler, splitter, KNN, metrics)
- **Concepts**:
  - Supervised Learning
  - Feature Scaling
  - Train-Test Split
  - K-Nearest Neighbors Algorithm
  - Model Evaluation (Accuracy, F1, Confusion Matrix)
- **IDE/Editor**: Visual Studio Code / Any Python-supported IDE

---

## 🚀 🚀 Code
- **Objectives**:

  - In this code we are going to build a Data Classification model using AI.
  - Our main Goal is to train a KNN classifier on the Iris dataset and evaluate its performance.
  - **Key Requirements** are: load and understand the dataset, split data into training and testing sets, apply a classification algorithm.
  - In this code we learn the concepts of data handling, supervised learning basics, and model training.

- **Explanation**:

  - Firstly, we import all required libraries — numpy, pandas, matplotlib, seaborn, and scikit-learn modules.
  - After that we load the Iris dataset using **load_iris()** and convert it into a pandas DataFrame for easy exploration.
  - Then we apply **StandardScaler** to normalize all features so that no single feature dominates due to scale differences.
  - After scaling, we split the data into 80% training and 20% testing sets using **train_test_split()** with shuffle and stratify enabled to remove order bias and maintain class balance.
  - We then use the Elbow Method — looping through K values from 1 to 30, training a KNN model for each, and recording the error rate to find the optimal K.
  - The final KNN model is trained using the optimal K found, then used to predict labels on the test set.
  - Output validation is performed by computing accuracy score, weighted F1 score, a full classification report, and a confusion matrix.
  - Three plots are generated and saved: an Elbow Curve showing error vs K, a Confusion Matrix heatmap, and a Feature Scatter plot of petal dimensions.
  - At the end, a Live Prediction Demo passes a new custom flower sample through the trained model and prints the predicted species with confidence probabilities.

## 🔧 Future Enhancements

- Add support for:
  - Other classification algorithms (Decision Tree, SVM, Random Forest)
  - Cross-validation for more robust evaluation
  - GUI integration using Tkinter or a web-based frontend
- Load custom datasets from a CSV file instead of the built-in Iris dataset
- Add hyperparameter tuning using GridSearchCV
- Deploy the model as a REST API using Flask or FastAPI

---
