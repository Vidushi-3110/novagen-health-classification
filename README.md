# 🏥 NovaGen Health Classification — Supervised ML

> **Assignment 5 | Prime AI Batch — Supervised Machine Learning**

Binary classification model to predict whether an individual is **Healthy** or **Unhealthy** based on health indicators — developed for NovaGen Research Labs.

---

## 📌 Problem Statement

NovaGen Research Labs conducts large-scale population health studies. The goal is to build a predictive model that classifies individuals as `Healthy (0)` or `Unhealthy (1)` using physiological, lifestyle, and medical history data — to support participant selection and risk stratification in clinical trials.

---

## 📊 Dataset

| Property | Value |
|----------|-------|
| Records  | 9,549 individuals |
| Features | 22 (numerical + categorical) |
| Target   | Binary (0 = Healthy, 1 = Unhealthy) |
| Missing Values | None |
| Class Balance | ~48% Healthy / ~52% Unhealthy |

### Features Used:
`Age`, `BMI`, `Blood_Pressure`, `Cholesterol`, `Glucose_Level`, `Heart_Rate`, `Sleep_Hours`, `Exercise_Hours`, `Water_Intake`, `Stress_Level`, `Smoking`, `Alcohol`, `Diet`, `MentalHealth`, `PhysicalActivity`, `MedicalHistory`, `Allergies`, `Diet_Type__Vegan`, `Diet_Type__Vegetarian`, `Blood_Group_AB`, `Blood_Group_B`, `Blood_Group_O`

---

## 🔧 Project Structure

```
novagen-health-classification/
│
├── novagen_health_classification.ipynb   # Main notebook (EDA + Models + Evaluation)
├── novagen_dataset.csv                   # Dataset
└── README.md
```

---

## 🚀 Models Trained & Compared

| Model | Description |
|-------|-------------|
| Logistic Regression | Linear baseline model |
| Decision Tree | Rule-based tree model |
| **Random Forest** ⭐ | Ensemble — best performer |
| Gradient Boosting | Boosting ensemble |
| KNN | Distance-based classifier |
| SVM | Support Vector Classifier |

---

## 📈 Workflow

1. **EDA** — Distribution plots, correlation heatmap, box plots
2. **Preprocessing** — Boolean encoding, StandardScaler, 80-20 train-test split
3. **Model Training** — 6 models compared on Accuracy, ROC-AUC, 5-Fold CV
4. **Evaluation** — Confusion matrix, classification report, ROC curves
5. **Feature Importance** — Top features identified via Random Forest
6. **Hyperparameter Tuning** — GridSearchCV on best model

---

## ▶️ How to Run

### Option 1: Google Colab (Recommended)
1. Upload `novagen_health_classification.ipynb` to [Google Colab](https://colab.research.google.com)
2. Upload `novagen_dataset.csv` when prompted
3. Run all cells (`Runtime > Run all`)

### Option 2: Local
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook novagen_health_classification.ipynb
```

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-2.x-blue?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.x-green)
![Seaborn](https://img.shields.io/badge/Seaborn-0.13-teal)

---

## 📚 Learnings

- End-to-end ML pipeline for binary classification
- Comparative model evaluation using multiple metrics
- Feature importance analysis
- Hyperparameter tuning with GridSearchCV

---

