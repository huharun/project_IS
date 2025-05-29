# 🛡️ Detecting Phishing Websites Using Machine Learning

This is a solo academic project by Arun Thangapalam for CSC 5800 – Intelligent Systems. The project focuses on detecting phishing websites using various machine learning algorithms applied to structured URL and domain metadata.

> Phishing is not just a nuisance — it’s a multi-billion dollar cybercrime. This project proves that classic ML still packs a punch in the fight against fakes.

---

## 📊 Project Overview

- Applied **11 different ML algorithms** to classify phishing vs. legitimate websites.
- Used a Kaggle dataset with **95,000+ records** and 10 numerical features.
- Conducted full **EDA, model training, evaluation, and visualization**.
- Ensemble models like **XGBoost**, **Random Forest**, and **AdaBoost** hit **>95% accuracy**.
- Visualized results with confusion matrices, ROC curves, feature importance, and decision tree plots.

---

## 🧠 Models Trained

| Type                | Algorithms                                   |
|---------------------|----------------------------------------------|
| Linear Models       | Logistic Regression, Linear SVM (SGD)        |
| Tree-Based          | Decision Tree, Random Forest, XGBoost        |
| Ensemble            | Bagging, AdaBoost                            |
| Probabilistic       | Naive Bayes                                   |
| Distance-Based      | K-Nearest Neighbors                           |
| Deep Learning       | MLP Neural Network                            |
| Kernel-Based        | SVM (RBF Kernel)                              |

---

## 📁 Files Included

- `det_phi_web.ipynb`: Jupyter notebook with full implementation
- `combined_dataset.csv`: Dataset used for training/testing
- `README.md`: You're reading it!
- 📽️ [Video Presentation](https://drive.google.com/file/d/1Z_PGcmBdlCZjM5OkBawRWuky01Ji9-3l/view?usp=drive_link)

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/phishing-ml.git
   cd phishing-ml
