<div align="center">

# 🔥 Project Phoenix

### Heart Disease Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0+-orange?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0+-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-1.24+-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12+-blue?style=for-the-badge)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7+-blue?style=for-the-badge)
![Accuracy](https://img.shields.io/badge/Accuracy-89%25-brightgreen?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)
![Day](https://img.shields.io/badge/30--Day--Challenge-Day%2015-red?style=for-the-badge)

<br/>

> A machine learning project that predicts the presence of heart disease in patients with **89% accuracy** using Logistic Regression — built as part of a 30-Day ML Challenge.

</div>

---

## 📌 Table of Contents

- [About the Project](#-about-the-project)
- [Dataset](#-dataset)
- [Project Structure](#-project-structure)
- [Pipeline](#-pipeline)
- [Results](#-results)
- [Key Insights](#-key-insights)
- [How to Run](#-how-to-run)
- [Libraries Used](#-libraries-used)
- [Author](#-author)

---

## 🧠 About the Project

Heart disease is one of the leading causes of death worldwide. Early and accurate prediction can save lives. This project builds a full ML pipeline — from raw data to a saved model — that predicts whether a patient has heart disease based on clinical features.

---

## 📊 Dataset

- **Source:** [Kaggle Heart Disease Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)
- **Rows:** 918 patients
- **Target Column:** `HeartDisease` (0 = No Disease, 1 = Disease)
- **Features:** Age, Sex, ChestPainType, RestingBP, Cholesterol, FastingBS, RestingECG, MaxHR, ExerciseAngina, Oldpeak, ST_Slope

---

## 📁 Project Structure

```
PROJECT-PHEONIX/
│
├── heart.csv               # Dataset
├── main.py                 # Main pipeline code
├── heart_model.pkl         # Saved trained model
└── README.md               # Project documentation
```

---

## ⚙️ Pipeline

```
RAW DATA
    │
    ▼
Data Loading & Inspection
    │
    ▼
Data Cleaning
  → Zero values in RestingBP & Cholesterol replaced with median
    │
    ▼
Exploratory Data Analysis
  → CountPlot  |  Histogram  |  BoxPlot  |  Heatmap
    │
    ▼
Feature Engineering
  → OneHotEncoding on 5 categorical columns
  → StandardScaling on all features
    │
    ▼
Model Training
  → Logistic Regression
    │
    ▼
Evaluation
  → Accuracy Score | Classification Report | Confusion Matrix
    │
    ▼
Model Saved → heart_model.pkl
```

---

## 📈 Results

| Metric | Score |
|--------|-------|
| **Accuracy** | **89%** |
| Precision (No Disease) | 0.87 |
| Precision (Disease) | 0.91 |
| Recall (No Disease) | 0.91 |
| Recall (Disease) | 0.88 |
| F1-Score (No Disease) | 0.89 |
| F1-Score (Disease) | 0.90 |

### Confusion Matrix

```
              Predicted
              0      1
Actual  0  [ 78     8  ]
        1  [ 11     87 ]
```

---

## 🔍 Key Insights

- **ASY (Asymptomatic)** chest pain is the most dangerous type — highest correlation with heart disease
- **Oldpeak** has the strongest positive correlation with heart disease (0.4)
- **MaxHR** has the strongest negative correlation with heart disease (-0.4)
- Heart disease risk increases significantly **after age 50**
- **Cholesterol** alone is a weak predictor (0.043 correlation)

---

## 🚀 How to Run

**1. Clone the repository**
```bash
git clone https://github.com/Boosterboy12/PROJECT-PHEONIX
cd PROJECT-PHEONIX
```

**2. Install dependencies**
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

**3. Run the project**
```bash
python main.py
```

---

## 📦 Libraries Used

| Library | Purpose |
|---------|---------|
| `NumPy` | Numerical operations |
| `Pandas` | Data manipulation |
| `Matplotlib` | Plotting |
| `Seaborn` | Advanced visualizations |
| `Scikit-learn` | ML pipeline, encoding, scaling, modeling |
| `Pickle` | Model saving |

---

## 👨‍💻 Author

**Vihaan** — Day 15 of 30-Day ML Challenge 🔥

[![GitHub](https://img.shields.io/badge/GitHub-Boosterboy12-black?style=for-the-badge&logo=github)](https://github.com/Boosterboy12)
[![Repository](https://img.shields.io/badge/Repo-PROJECT--PHEONIX-blue?style=for-the-badge&logo=github)](https://github.com/Boosterboy12/PROJECT-PHEONIX)

---

<div align="center">
  <i>Built with 🔥 as part of the 30-Day ML Challenge</i>
</div>
