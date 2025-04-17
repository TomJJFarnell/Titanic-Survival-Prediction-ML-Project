# Titanic-Survival-Prediction-ML-Project
Predicting survival on the Titanic using machine learning. A beginner-friendly classification project using data cleaning, feature engineering, and model training (Logistic Regression, Random Forest, XGBoost).


# 🚢 Titanic Survival Prediction: Machine Learning Project

A complete end-to-end machine learning project using the classic Titanic dataset. This notebook demonstrates data cleaning, exploratory analysis, feature engineering, and training multiple ML models to predict passenger survival.

---

## 📦 Dataset

- Source: [Kaggle Titanic Competition](https://www.kaggle.com/c/titanic)
- Format: CSV
- Key columns: `Pclass`, `Sex`, `Age`, `SibSp`, `Fare`, `Embarked`, `Survived`

---

## 🧰 Tools & Libraries

- Python
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- XGBoost (optional)

---

## 🧹 Data Cleaning

- Handled missing values in `Age`, `Embarked`, and `Cabin`
- Converted categorical variables (`Sex`, `Embarked`) into numeric form
- Removed outliers and unnecessary columns

---

## 📊 Exploratory Data Analysis (EDA)

- Survival rate by gender, class, age, and embarkation point
- Distribution plots and heatmaps to visualize correlations

---

## 🛠️ Feature Engineering

- Created new features like `FamilySize`, `IsAlone`, and `Title`
- Binned age and fare into categories for better modeling
- One-hot encoded categorical variables

---

## 🤖 Model Training & Evaluation

Tested multiple ML models:

| Model              | Accuracy Score |
|--------------------|----------------|
| Logistic Regression| 78%            |
| Random Forest      | 81%            |
| XGBoost            | 82%            |

- Used train/test split for validation
- Cross-validated results
- Confusion matrix and classification report for final evaluation

---

## 📈 Results

XGBoost gave the best performance with an accuracy of **~82%**, outperforming baseline models. Feature importance showed `Sex`, `Pclass`, and `Fare` were the most influential factors in predicting survival.

