# Student Math Performance Prediction

A machine learning project that predicts whether a student will pass or fail in Math based on demographic and academic factors.

---

## About the Project

This project uses the Students Performance dataset to build a binary classification model. A student is classified as **Pass** if their math score is 40 or above, and **Fail** otherwise. The goal is to identify key factors that influence math performance.

---

## Dataset

- **File:** `exams.csv`
- **Records:** 1000 students
- **Features:**
  - Gender
  - Race/Ethnicity
  - Parental Level of Education
  - Lunch Type
  - Test Preparation Course
  - Reading Score
  - Writing Score
- **Target:** `pass_math` (1 = Pass, 0 = Fail)

---

## Workflow

1. Loaded and explored the dataset
2. Created target column based on math score threshold (≥ 40 = Pass)
3. Performed EDA — Pass/Fail distribution, correlation heatmap
4. Label encoded categorical columns
5. Split data into 80% train and 20% test
6. Trained a Logistic Regression model
7. Evaluated using Accuracy, Confusion Matrix, and Classification Report

---

## Tech Stack

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

## Results

### Logistic Regression
| Metric | Value |
|--------|-------|
| Accuracy | 97.5% |
| Precision (Pass) | 0.98 |
| Recall (Pass) | 0.99 |
| F1-Score (Pass) | 0.99 |

> **Note:** The dataset is heavily imbalanced — 193 students passed vs only 7 failed. Due to this imbalance, the model achieves high overall accuracy but performs poorly on the minority class (Fail — Recall: 43%). A balanced dataset or techniques like SMOTE would likely produce more reliable results.

---

*Developed by Prince Joshi | Aspiring Data Analyst*
