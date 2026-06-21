# 🏡 House Price Prediction using Machine Learning

## 📌 Project Overview

This project predicts residential house prices using the **Ames Housing Dataset**. The workflow includes data preprocessing, feature engineering, model training, hyperparameter tuning, and evaluation using multiple regression metrics.

The entire machine learning pipeline was built using **Scikit-learn Pipelines** and **ColumnTransformer**, ensuring clean, reproducible preprocessing without data leakage.

---

## 🚀 Features

* Data Cleaning & Missing Value Handling
* Feature Engineering
* Categorical Encoding using One-Hot Encoding
* Numerical Feature Scaling
* End-to-End Scikit-learn Pipeline
* Gradient Boosting Regressor
* Hyperparameter Tuning using GridSearchCV
* Model Evaluation using Multiple Metrics

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn

---

## 📊 Dataset

* **Dataset:** Ames Housing Dataset
* **Rows:** 2,930
* **Target Variable:** `SalePrice`

The dataset contains information about house characteristics including:

* Property Size
* Basement Features
* Garage Information
* Interior Quality
* Neighborhood
* Sale Details

---

## 🔧 Data Preprocessing

### Missing Value Handling

* Numerical columns → Median Imputation
* Categorical columns → Most Frequent Imputation

### Encoding

* One-Hot Encoding for categorical variables
* Unknown categories handled using `handle_unknown="ignore"`

### Scaling

* StandardScaler applied to numerical features

---

## 🧠 Feature Engineering

The following custom features were created to improve model performance:

* `ageofhouse = Yr Sold - Year Built`
* `TotalBath`
* `TotalPorchSF`
* `TotalFinishedSF`
* `YearsSinceRemodel`
* `HasGarage`
* `HasBasement`
* `Remodeled`

---

## 🤖 Machine Learning Model

Model used:

* Gradient Boosting Regressor

Hyperparameter tuning was performed using **GridSearchCV** with **5-fold Cross Validation**.

Parameters tuned:

* Number of Estimators
* Learning Rate
* Maximum Tree Depth
* Minimum Samples Split
* Minimum Samples Leaf
* Subsample Ratio

---

## 📈 Model Performance

Evaluation Metrics:

* R² Score
* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)

Example Results:

| Metric   | Value   |
| -------- | ------- |
| R² Score | 0.923   |
| MAE      | ~15,000 |
| RMSE     | ~24,800 |

---



## ▶️ How to Run

1. Clone the repository

```bash
git clone <repository-link>
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Open the notebook or run the Python script.

---

## 📌 Key Learnings

* Data preprocessing with Scikit-learn Pipelines
* Handling missing values effectively
* Feature engineering for regression problems
* Hyperparameter tuning using GridSearchCV
* Cross-validation for model selection
* Building reproducible machine learning workflows

---

## 📜 License

This project is for educational and portfolio purposes.
