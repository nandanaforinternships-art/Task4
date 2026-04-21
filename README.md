# Task4 

# Logistic Regression Binary Classifier

## Project Overview

This project implements a **Logistic Regression model** for binary classification using the **Breast Cancer Wisconsin dataset**.
The goal is to classify tumors as **malignant (0)** or **benign (1)** based on input features.

---

## Features

* Data preprocessing (train-test split + feature scaling)
* Logistic Regression model training
* Model evaluation using:

  * Confusion Matrix
  * Precision & Recall
  * ROC-AUC Score
* ROC Curve visualization
* Threshold tuning for performance optimization

---

## Dataset

The dataset is loaded from `sklearn.datasets`:

* **Breast Cancer Wisconsin Dataset**
* 569 samples
* 30 numerical features
* Binary classification:

  * `0 = Malignant`
  * `1 = Benign`

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn

---

## Model Workflow

1. Load dataset
2. Split into training and testing sets
3. Apply feature scaling using StandardScaler
4. Train Logistic Regression model
5. Make predictions
6. Evaluate performance
7. Plot ROC Curve
8. Tune classification threshold

---

## Evaluation Metrics

* **Confusion Matrix** – Shows prediction accuracy
* **Precision** – Correct positive predictions
* **Recall** – Coverage of actual positives
* **ROC-AUC Score** – Overall model performance

---

## Logistic Function

The Logistic Regression model uses the sigmoid function:

[
\sigma(z) = \frac{1}{1 + e^{-z}}
]

This converts output into probabilities between 0 and 1.

## Output

* Printed evaluation metrics in console
* ROC Curve visualization
* Confusion matrix results
* Performance comparison with different thresholds

---

## Threshold Tuning

By default, classification threshold = **0.5**

You can modify it to improve:

* **Lower threshold → Higher recall**
* **Higher threshold → Higher precision**
