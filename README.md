
# ❤️ Heart Failure Prediction (Machine Learning)

A compact ML project that predicts the likelihood of **death events** in heart-failure patients using clinical features. The work is implemented in a single Jupyter Notebook and evaluates multiple classification models with class-imbalance handling.

## 📂 Project Contents

```
.
├── Heart_failure_prediction (1).ipynb   # Main notebook (training & evaluation)
├── heart_failure_clinical_records.csv   # Dataset (place alongside the notebook)
└── README.md                            # This file
```

## 🎯 Objective

Predict the target **`DEATH_EVENT`** (0 = survived, 1 = died during follow-up) from routinely collected clinical variables.

Typical features in this dataset include (not exhaustive):
`age, anaemia, creatinine_phosphokinase, diabetes, ejection_fraction, high_blood_pressure, platelets, serum_creatinine, serum_sodium, sex, smoking, time`.

---

## 🛠️ What’s in the Notebook

### Data & Split

* Loads: `heart_failure_clinical_records.csv`
* Target: **`DEATH_EVENT`**
* Train/test split: **80/20**, with **stratification** and `random_state=42`.

### Models Trained

* **LogisticRegression**
* **Support Vector Machine (SVM)**
* **DecisionTreeClassifier**
* **RandomForestClassifier**

### Metrics & Visuals

* **Accuracy** on train and test sets for each model
* **Confusion matrix** & **classification report** for the selected/best model
* Bar chart comparing model accuracies

---

## 📊 Results 

> Test accuracies reported in the notebook:

| Model               | Test Accuracy |
| ------------------- | ------------- |
| Logistic Regression | **0.783**     |
| SVM                 | **0.626**     |
| Decision Tree       | **0.986**     |
| Random Forest       | **0.993**     |

**Best performer:** RandomForestClassifier (≈ **99.3%** test accuracy in this run)

---
