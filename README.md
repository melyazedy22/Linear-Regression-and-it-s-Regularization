# Linear-Regression-and-it-s-Regularization
# 🚗 Used Cars Price Prediction (Regularization Practice) ((( Session 2 in ML)))

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
This project focuses on **predicting the prices of used cars** using Machine Learning. It serves as a practical application of **Regularization techniques (L1 Lasso & L2 Ridge)** to improve the performance of Linear Regression models and prevent overfitting, ensuring more reliable price estimates.

## 🛠️ Workflow & Methodology

### 1. Data Preprocessing
* **Cleaning:** Handled missing values and ensured data consistency.
* **Encoding:**
    * **OneHotEncoder:** Applied to nominal categorical variables (e.g., car brand).
    * **LabelEncoder:** Applied to ordinal categorical variables (e.g., condition).

### 2. Modeling Strategy
The project explores multiple regression approaches to find the best fit:
* **Linear Regression:** Trained as a baseline model to establish initial performance.
* **Lasso Regression (L1):** Implemented to perform feature selection by shrinking less important coefficients to zero.
* **Ridge Regression (L2):** Implemented to handle multicollinearity and stabilize coefficient estimates.

### 3. Hyperparameter Tuning
* **GridSearchCV:** Used to systematically search for the optimal `alpha` hyperparameter for both Lasso and Ridge models, balancing bias and variance.

## 📊 Results
* **Best Model Accuracy (R² Score):** The tuned model achieved an R² score of **~86%**, indicating a strong predictive capability.
* **Optimal Configuration:** The GridSearch identified **0.001** as the best `alpha` value for the regularization term.

## ⚙️ Technologies Used
* **Python**
* **Pandas & NumPy** (Data Manipulation)
* **Scikit-Learn** (Modeling, Preprocessing, Model Selection)

## 🚀 How to Run
1.  **Clone the repository** (or download the files).
2.  **Install requirements:**
    ```bash
    pip install pandas numpy scikit-learn
    ```
3.  **Launch Jupyter Notebook:**
    ```bash
    jupyter notebook "Used_Cars_Practice+L1&L2 Regularization .ipynb"
    ```
