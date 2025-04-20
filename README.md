# AIML-Module-5-Data-Evaluation: Used Car Price Driver Analysis

## OVERVIEW:

This project explores a dataset of used car listings to understand the key factors that influence vehicle prices. The analysis aims to provide actionable insights for a used car dealership regarding consumer preferences and valuable vehicle characteristics.

The original dataset from Kaggle contained information on 3 million used cars. For computational efficiency, this project utilizes a subset containing data on approximately 426,000 cars.

**Project Goal:** To identify the main drivers of used car prices and provide recommendations for inventory management and pricing strategies based on what consumers value most in a used car.

## Technical Task:

The core task is to build and evaluate machine learning regression models (specifically Linear Regression, Lasso Regression, and Ridge Regression) to predict used car prices based on vehicle features. The analysis focuses on:

1.  **Data Cleaning & Preprocessing:**
    *   Handling missing values (NaNs and nulls).
    *   Dropping irrelevant columns that do not contribute to price prediction.
    *   Scaling numerical features (like year and odometer) for model compatibility.
    *   Encoding categorical features (like manufacturer, condition, type) appropriately, potentially using techniques like Target Encoding for high-cardinality features.

2.  **Modeling:**
    *   Training Linear, Lasso, and Ridge regression models.
    *   Employing `GridSearchCV` to tune hyperparameters, particularly the regularization strength (`alpha`) for Lasso and Ridge, to optimize model performance.

3.  **Evaluation:**
    *   Assessing model performance on unseen test data using standard regression metrics:
        *   Mean Absolute Error (MAE)
        *   Root Mean Squared Error (RMSE)
        *   R-squared (R²)

4.  **Driver Analysis:**
    *   Analyzing the coefficients of the trained models (especially the best-performing one) to determine the relative importance and impact (positive or negative) of different vehicle features on the predicted price.

## Business Objective:

The primary business objective is to leverage data analysis to understand consumer valuation drivers for used cars. By identifying which vehicle characteristics (e.g., age, mileage, condition, make) most significantly impact market price, the dealership can make more informed decisions regarding:

*   **Inventory Acquisition:** Focusing on acquiring vehicles with characteristics that command higher prices or offer better value.
*   **Pricing Strategy:** Setting prices that accurately reflect the market value based on key features.

## Project Structure:

The analysis is conducted within a Jupyter Notebook (`prompt_II.ipynb`) following a structured approach, likely mirroring the CRISP-DM framework:

1.  **Business Understanding:** Defining the problem and objectives (as outlined above).
2.  **Data Understanding:** Initial exploration, visualization, and identification of data quality issues.
3.  **Data Preparation:** Cleaning, imputation, feature engineering, scaling, and encoding.
4.  **Modeling:** Training and tuning regression models.
5.  **Evaluation:** Assessing model performance and comparing different models.
6.  **Deployment:** Summarizing findings and providing actionable recommendations (represented by the final report section in the notebook).

## Dependencies:

The analysis uses standard Python data science libraries, including:

*   pandas
*   numpy
*   matplotlib
*   seaborn
*   scikit-learn (for models, preprocessing, metrics, GridSearchCV)
*   category_encoders (specifically for TargetEncoder)

---

*Readme generated with assistance from Google AI.*
