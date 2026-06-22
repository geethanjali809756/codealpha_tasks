# Disease Prediction from Medical Data

A machine learning project to predict the possibility of diseases based on patient medical data, developed as part of the **CodeAlpha Machine Learning Internship**.

---

## Overview

This project covers prediction of three diseases — **Heart Disease**, **Diabetes**, and **Breast Cancer** — using multiple classification algorithms. Each disease is treated as a separate binary classification problem, with models trained, compared, and evaluated independently.

---

## Datasets

| Disease | Dataset | Source |
|---------|---------|--------|
| Heart Disease | UCI Cleveland Heart Disease | UCI ML Repository (auto-downloaded) |
| Diabetes | Pima Indians Diabetes | GitHub mirror (auto-downloaded) |
| Breast Cancer | Breast Cancer Wisconsin | Scikit-learn built-in |

No manual download required — all datasets load automatically when the notebook runs.

---

## Technologies Used

- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn, XGBoost
- Google Colab / Jupyter Notebook

---

## Models Used

- Logistic Regression
- Random Forest Classifier
- Support Vector Machine (SVM)
- Gradient Boosting Classifier
- XGBoost Classifier

---

## Project Workflow

1. Load datasets automatically via URL or sklearn
2. Exploratory Data Analysis (EDA) and visualizations
3. Data preprocessing and feature scaling
4. Train and compare multiple models per disease
5. Evaluate using Accuracy, F1 Score, ROC-AUC, and Cross-Validation
6. Predict on new patient data
7. Save all trained models as `.pkl` files

---

## Evaluation Metrics

Models are evaluated using Accuracy, Precision, Recall, F1 Score, ROC-AUC Score, and 5-Fold Cross-Validation.

---

## Getting Started

```bash
# Install dependencies
pip install xgboost scikit-learn pandas numpy matplotlib seaborn
```

Open the notebook in Google Colab and run all cells sequentially. All datasets are downloaded automatically — no setup needed.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/)

---

## Repository Structure

```
CodeAlpha_DiseasePrediction/
├── CodeAlpha_DiseasePrediction.ipynb
├── README.md
└── models/
    ├── heart_disease_model.pkl
    ├── heart_scaler.pkl
    ├── diabetes_model.pkl
    ├── diabetes_scaler.pkl
    ├── breast_cancer_model.pkl
    └── breast_cancer_scaler.pkl
```

---

## Outcome

The project successfully predicts disease risk for all three conditions. The best-performing model is selected automatically based on accuracy and used for new patient predictions.

---

## Author

**Geethanjali**  
CodeAlpha Machine Learning Internship
