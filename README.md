# Linear-Regression-and-it-s-Regularization
---
# 📈 Linear Regression Practice: OLS & Gradient Descent *(Session 1 in ML)*

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview
This project demonstrates the implementation of **Linear Regression** using two different approaches: **Ordinary Least Squares (OLS)** via Scikit-Learn and a manual implementation of **Gradient Descent**. The goal is to predict student performance (GPA) based on SAT scores, providing a clear comparison between the analytical and iterative methods of regression.



[Image of simple linear regression plot]


## 🛠️ Workflow & Methodology

### 1. Data Preprocessing
* **Dataset:** USA Student Data (SAT scores vs. GPA).
* **Cleaning:** Checked for missing values and ensured data integrity.
* **Visualization:** Plotted scatter charts to visualize the positive correlation between SAT scores and GPA.

### 2. Modeling Approaches
* **Ordinary Least Squares (OLS):**
    * Implemented using `sklearn.linear_model.LinearRegression`.
    * Solves for the best-fitting line analytically.
* **Gradient Descent (Manual Implementation):**
    * Developed a custom function to iteratively update the regression coefficients (slope `m` and intercept `c`).
    * Minimized the Cost Function (Mean Squared Error) over multiple epochs.
* **Polynomial Regression:**
    * Experimented with `PolynomialFeatures` (Degree 2) to capture non-linear relationships.

### 3. Evaluation & Visualization
* **Metrics:** Evaluated models using R² Score and coefficients (Slope & Intercept).
* **Plots:**
    * **Regression Line:** Visualized the best-fit line over the training data.
    * **Loss Curve:** Plotted the cost function over iterations to verify convergence in Gradient Descent.

## 📊 Results
* **Convergence:** The Gradient Descent algorithm successfully converged, producing coefficients very close to the Scikit-Learn OLS solution.
* **Polynomial Fit:** The Degree 2 polynomial model provided a slightly flexible curve, potentially capturing subtle non-linearities in the SAT-GPA relationship.

## ⚙️ Technologies Used
* **Python**
* **Pandas & NumPy** (Data Manipulation & Math)
* **Matplotlib & Seaborn** (Data Visualization)
* **Scikit-Learn** (OLS Modeling & Preprocessing)
---
---
---
# 🚗 Used Cars Price Prediction (Regularization Practice) *( Session 2 in ML)*

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


