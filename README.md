# Forest Fires Analysis

## Project Overview

This project analyzes the **Forest Fires** dataset from the UCI Machine Learning Repository to investigate the environmental factors associated with wildfire behavior. The primary objective is to identify the variables that influence wildfire size, develop predictive models for wildfire risk, and provide recommendations that can support wildfire prevention and resource allocation.

The analysis combines **exploratory data analysis (EDA)**, **multiple regression**, **regularization techniques**, and **binary classification** to evaluate different approaches for modeling wildfire behavior.

---

## Project Objectives

The project aims to:

* Analyze the factors that contribute to fire size and severity.
* Develop models capable of predicting high-risk areas.
* Provide actionable recommendations to aid in risk mitigation.

---

## Dataset

* **Dataset:** Forest Fires
* **Source:** UCI Machine Learning Repository
* **Observations:** 517 (513 after removing duplicate records)
* **Target Variable:** Burned area (`area`)

The dataset includes:

* Weather conditions (temperature, humidity, wind, rainfall)
* Fire Weather Index (FWI) variables
* Spatial coordinates
* Calendar variables (month and day)

---

## Project Workflow

The complete analysis is contained in **`CO6MO8Lab.ipynb`**, which follows this workflow:

* Load and inspect the dataset.
1. Perform Exploratory Data Analysis (EDA).
2. Clean the data by checking for missing values and duplicate observations.
3. Explore distributions, correlations, and outliers.
4. Build and evaluate multiple regression models:

   * Baseline Multiple Linear Regression
   * Nonlinear Regression
   * Regression with Interaction Terms
   * Regression with Indicator Variables
   * Log-Transformed Regression
5. Assess model assumptions using:

   * Residual Plots
   * Q-Q Plots
   * Cook's Distance
   * Variance Inflation Factor (VIF)
6. Apply Ridge and Lasso Regression.
7. Convert the problem into a binary classification task.
8. Train and evaluate a Logistic Regression model.
9. Compare model performance and provide business recommendations.

---

## Repository Structure

```text
.
├── C06M08Lab.ipynb                   # Complete workflow and analysis
├── Forest_Fires_Final_Report.pdf     # Final written report
├── README.md                         # Project documentation
```

---

## Models Implemented

### Regression Models

* Multiple Linear Regression
* Nonlinear Regression
* Interaction Model
* Indicator Variable Model
* Log-Transformed Regression
* Ridge Regression
* Lasso Regression

### Classification Model

* Logistic Regression

---

## Evaluation Metrics

Regression models were evaluated using:

* R²
* Adjusted R²
* F-statistic
* p-value
* AIC
* BIC
* Mean Squared Error (MSE)

Classification performance was evaluated using:

* Accuracy
* Confusion Matrix
* Precision
* Recall
* F1-score

Model assumptions were assessed using:

* Residual Plots
* Q-Q Plots
* Cook's Distance
* Variance Inflation Factor (VIF)

---

## Summary of Findings

The baseline multiple linear regression model provided the best balance between simplicity, interpretability, and statistical performance, although it explained only a small proportion of the variation in burned area. Ridge and Lasso regression produced similar results because multicollinearity among the predictors was low. Logistic regression achieved modest classification performance, indicating that the available predictors alone were insufficient for accurately distinguishing between low-risk and high-risk fires.

Overall, the analysis suggests that additional information, such as vegetation characteristics, fuel load, topography, and human activity, would likely improve predictive performance.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* SciPy
* Scikit-learn
* Statsmodels
* UCI Machine Learning Repository

---

## Author

**Fascos Jepleting**

---

