## Gender Classification Using Academic Scores

##  Project Overview

This machine learning project aims to classify the gender of students based on their performance in three academic subjects: Math, Reading, and Writing. The gender is encoded as a binary variable — `0` for male and `1` for female — and classification models are used to predict this label.

##  Problem Statement

Can a student's gender be predicted accurately based on their exam scores? This project investigates the viability of such a prediction using supervised classification algorithms and performance metrics.

##  Dataset

* **Source**: `exams.csv`
* **Features Used**:

  * Math Score
  * Reading Score
  * Writing Score
* **Target**: Gender (`0` = Male, `1` = Female)
* **Data Cleaning**:

  * Irrelevant columns such as race/ethnicity, parental level of education, lunch, and test preparation course were removed.
  * Gender values were encoded to binary integers.

## Tools & Technologies

* **Programming Language**: Python
* **Libraries**:

  * `pandas`, `numpy` – Data handling
  * `seaborn`, `matplotlib` – Visualization
  * `scikit-learn` – Machine learning models and metrics
  * `statsmodels` – Statistical evaluation

## Methodology

1. **Data Preprocessing**:

   * Dropped irrelevant features
   * Normalized feature values using `StandardScaler`
   * Encoded gender column for binary classification

2. **Model Selection & Evaluation**:

   * Multiple classification algorithms were tested:

     * Logistic Regression
     * Decision Tree Classifier
     * Random Forest Classifier
     * Support Vector Machine (SVM)
     * K-Nearest Neighbors (KNN)
     * Gaussian Naive Bayes
   * 5-fold Cross Validation was used to split the data
   * Evaluation Metrics:

     * Accuracy Score
     * Confusion Matrix
     * Classification Report (Precision, Recall, F1-score)
     * ROC Curve & AUC Score

##  Decision Criteria

Decisions in this project were made based on:

* **Cross-validated Accuracy Score** across models
* **Confusion Matrix Analysis** (True Positive, False Positive, etc.)
* **ROC AUC Score**, which measures model performance across thresholds
* Preference for models with better generalization and less overfitting

##  Results Summary

* Each model was evaluated using consistent cross-validation and metric calculations.
* Performance was visualized using confusion matrices and ROC curves.
* Model accuracy varied depending on the algorithm, with tree-based models and logistic regression showing relatively higher AUC and balanced precision-recall.

##  Key Learning

This project demonstrates how basic academic scores can be used as predictors in binary classification problems. It also shows the importance of evaluating multiple algorithms using cross-validation and different performance metrics rather than relying on accuracy alone.


