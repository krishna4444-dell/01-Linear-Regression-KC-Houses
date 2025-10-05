# House Price Prediction using Linear Regression

##  Project Overview

This project applies **Linear Regression** to predict house prices using the **King County Housing dataset**. The dataset contains house sales data including features like square footage, number of bedrooms/bathrooms, grade, view, etc.

The main goal was to build a **Linear Regression model**, evaluate its performance, and interpret the coefficients to understand which features influence house prices the most.

---

## Steps Followed

1. **Exploratory Data Analysis (EDA)**

   * Checked dataset info, missing values, and descriptive stats.
   * Correlation analysis to find most important features.
   * Visualizations (scatterplots, heatmaps).

2. **Feature Selection**

   * Selected top correlated features (`sqft_living`, `grade`, `view`).
   * Checked multicollinearity using **Variance Inflation Factor (VIF)**.

3. **Linear Regression Model**

   * Implemented **Simple Linear Regression** with one feature.
   * Extended to **Multiple Linear Regression** with selected features.
   * Evaluated performance with R², RMSE, and cross-validation.

4. **Model Evaluation**

   * Train/Test split performance.
   * **Cross-validated R²:** ~0.57
   * Coefficient interpretation:

     * Each extra sqft adds ~$168.
     * Each increase in grade adds ~$91k.
     * Better view adds ~$96k.

5. **Residual Analysis**

   * Residual plots showed errors are fairly random, but model doesn’t capture all variability.

---

##  Results

* Final model explains **~57% of house price variation**.
* sqft_living,grade,and view are the strongest predictors.
* Linear Regression provides a solid baseline but more advanced models (Ridge, Lasso, Random Forest, XGBoost) could improve accuracy.

---

##  How to Run

1. Clone this repo:
 
2.git clone https://github.com/<your-username>/01-Linear-Regression-KC-Houses.git

3. Install dependencies:

   pip install -r requirements.txt
  
4. Open the Jupyter/Colab notebook and run all cells.

---

##  Future Work

* Apply **Regularization (Ridge/Lasso)** to handle multicollinearity.
* Try **Polynomial Features** to capture non-linear trends.
* Explore **Tree-based models** for better accuracy.

---

##  Author

Name: Krishna Kishore
Email:pilagalakrishnakishore@gmail.com
LinkedIn:www.linkedin.com/in/pilagala-krishna-kishore-423146355

---
