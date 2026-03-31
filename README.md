\# Annual Salary Estimation for Banking Customers



\## 📌 Project Overview

This repository contains a comprehensive Jupyter Notebook (`(Regression) LR+KNN+RF+Boosting Models.ipynb`) that demonstrates an end-to-end regression workflow for estimating the annual salary of banking customers. By leveraging transaction-level data, the project aggregates financial behaviors—such as spending patterns, balance averages, and credit/debit movements—to predict a customer's income level.



The project evaluates a variety of machine learning algorithms, ranging from traditional linear models to advanced gradient-boosted decision trees, to identify the most accurate approach for salary prediction.



\## 🛠️ Project Workflow

The notebook follows a structured end-to-end data science pipeline:



1\.  \*\*Library Integration\*\*: 

&#x20;   \* Loading essential data science and machine learning libraries including Scikit-Learn, XGBoost, LightGBM, CatBoost, and Optuna for hyperparameter tuning.

2\.  \*\*Feature Engineering \& Aggregation\*\*: 

&#x20;   \* Transforming raw transaction data into customer-level features such as average balance, transaction frequency, and total salary recorded.

3\.  \*\*Data Cleaning\*\*: 

&#x20;   \* Handling missing values and ensuring data consistency across aggregated features.

4\.  \*\*Outlier Treatment\*\*: 

&#x20;   \* Implementation of outlier capping (\*\*Winsorization\*\*) to prevent extreme financial transactions from skewing the regression results.

5\.  \*\*Multicollinearity Analysis\*\*: 

&#x20;   \* Using \*\*Variance Inflation Factor (VIF)\*\* to detect and remove highly correlated features, ensuring the stability of the regression models.

6\.  \*\*Data Preprocessing\*\*: 

&#x20;   \* \*\*Scaling\*\*: Applying `StandardScaler` for feature normalization.

&#x20;   \* \*\*Encoding\*\*: Using `LabelEncoder` for categorical variables to prepare the data for distance-based and linear algorithms.

7\.  \*\*Modeling \& Optimization\*\*:

&#x20;   \* \*\*Baseline Models\*\*: Linear Regression and KNN to establish initial performance.

&#x20;   \* \*\*Tree-Based Models\*\*: Training Random Forest, XGBoost, LightGBM, and CatBoost.

&#x20;   \* \*\*Hyperparameter Tuning\*\*: Utilizing \*\*Optuna\*\* to find the optimal parameters for the boosting models.

8\.  \*\*Model Evaluation\*\*: 

&#x20;   \* Comparing models using a suite of regression metrics: MAE, MSE, RMSE, $R^2$, and Adjusted $R^2$.



\## ⚠️ Methodology \& Computational Constraints

\* \*\*Task-Related Thresholds\*\*: Please note that some thresholds and parameters used in this notebook (such as specific VIF cut-off points or outlier boundaries) were determined based on \*\*specific task requirements\*\*. These may differ from standard industry "best practices" depending on the specific analytical goals and risk appetite of a given institution.

\* \*\*Hardware Limitations\*\*: Because the tree-based models (Random Forest, XGBoost, etc.) were trained on a local machine, model performances may be "not ideal." The depth of hyperparameter grid searches and the number of iterations were constrained by available computational resources.



\## 💻 Technologies Used

\- \*\*Python 3.x\*\*

\- \*\*Data Analysis\*\*: Pandas, NumPy

\- \*\*Visualization\*\*: Matplotlib, Seaborn

\- \*\*Machine Learning\*\*: Scikit-Learn, XGBoost, LightGBM, CatBoost

\- \*\*Optimization\*\*: Optuna

\- \*\*Statistical Analysis\*\*: Statsmodels (VIF), SciPy (Stats)



\## 🚀 How to Use

1\. Ensure you have the dataset file (`income\_est.xlsx`) in the same directory as the notebook.

2\. Install the required dependencies:

&#x20;  ```bash

&#x20;  pip install pandas numpy seaborn matplotlib scikit-learn statsmodels optuna xgboost lightgbm catboost openpyxl

&#x20;  ```

3\. Run the notebook using Jupyter Lab, Jupyter Notebook, or VS Code.



\---

\*Created as part of a professional development exercise in Financial Data Science.\*

