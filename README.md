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

| Metric | Value |
|--------|-------|
| Model | Logistic Regression |
| Train/Test Split | 80/20 |

---

*Developed by Prince Joshi | Aspiring Data Analyst*
