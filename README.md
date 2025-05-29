# Phishing Website Detection Using Machine Learning

This project presents a machine learning-based approach to detecting phishing websites using structured URL and domain-level features. Developed as an individual academic project for the CSC 5800 – Intelligent Systems course, it demonstrates the feasibility of using traditional ML models to address real-world cybersecurity challenges.

## Project Overview

Phishing websites imitate legitimate platforms in order to deceive users into providing sensitive information. This project utilizes a Kaggle dataset of over 95,000 entries and applies 11 machine learning algorithms to classify websites as phishing or legitimate. The models were evaluated using standard metrics such as accuracy, precision, recall, F1 score, confusion matrices, and ROC curves.

## Objectives

- Apply multiple supervised learning algorithms to phishing detection
- Perform comprehensive exploratory data analysis (EDA)
- Evaluate model performance across various statistical metrics
- Interpret results using visual tools such as ROC curves and feature importance
- Identify the most effective models and features for deployment

## Models Implemented

The following algorithms were trained and compared:

- Logistic Regression
- Decision Tree
- Random Forest
- Tuned Random Forest (GridSearch)
- XGBoost
- AdaBoost
- Naive Bayes
- K-Nearest Neighbors
- Support Vector Machine (RBF Kernel)
- Linear SVM (SGD)
- Multi-Layer Perceptron (Neural Network)

## Dataset

- Source: Kaggle – Phishing Website Detector
- Total Records: 95,910
- Features: 10 numeric/binary predictors
- Target: Binary label (1 = phishing, 0 = legitimate)

The dataset was clean, with no missing values. All features were already numeric.

## Exploratory Data Analysis

EDA revealed the following:

- Phishing URLs tend to be longer and often include symbols such as dashes
- Key predictive features include `urlLen`, `ranking`, and `haveDash`
- The dataset is balanced, reducing bias in training

## Preprocessing

- Dropped non-numeric columns (e.g., domain name)
- Normalized features using `StandardScaler` for models sensitive to scale
- Split the dataset into training and test sets (80/20)

## Evaluation Metrics

Each model was evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC Curve and AUC Score

## Key Results

- Ensemble methods (Random Forest, AdaBoost, XGBoost) outperformed others
- XGBoost achieved the highest accuracy and AUC score
- Feature importance rankings consistently highlighted `urlLen`, `ranking`, and `haveDash`

## Visualizations

The following plots were used to interpret model behavior:

- Confusion matrices (grid comparison)
- ROC curves with AUC scores
- Decision tree visualization
- Feature importance charts

## Future Work

- Incorporate text-based analysis of domain and URL strings
- Use HTML and JavaScript content for content-based phishing detection
- Explore deep learning architectures such as LSTMs and Transformers
- Integrate with real-time threat intelligence feeds (e.g., PhishTank)
- Deploy as a browser extension or REST API for real-time protection

## How to Run

To run this project locally:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/phishing-ml.git
   cd phishing_IS
