
# 🏠 Real Estate Price Prediction

A machine learning project that predicts real estate property prices based on key features such as location, number of bedrooms, size (square feet), and amenities. Built using Python, Pandas, Scikit-learn, and Jupyter Notebook.
Data Source : https://www.kaggle.com/datasets/shubheshswain/bangalore-house-price-data

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Tech Stack](#tech-stack)
- [Dataset](#dataset)
- [Workflow](#workflow)
- [Modeling](#modeling)
- [Results](#results)


## 📈 Project Overview

This project aims to predict the prices of residential properties using regression models. It is designed as a practical implementation of exploratory data analysis (EDA), feature engineering, and model training for tabular data in the real estate domain.

> Goal: Given features like location, number of bedrooms, total square footage, and bathrooms, accurately predict the property price.

## 🛠 Tech Stack

- Python 3.x
- Jupyter Notebook
- NumPy, Pandas, Matplotlib, Seaborn
- Scikit-learn
- Pickle (for model saving)

## 📊 Dataset

The dataset used is derived from housing data in Bangalore, India (publicly available from Kaggle and other open sources).

**Key Features:**
- `location`
- `total_sqft`
- `bath`
- `bhk`
- `price`

## 🔁 Workflow

1. **Data Cleaning**
   - Handling missing values
   - Converting square feet to numeric
   - Removing outliers

2. **Feature Engineering**
   - Creating new features like `price_per_sqft`
   - Encoding categorical variables (e.g., `location`)

3. **Model Building**
   - Linear Regression
   - Lasso Regression
   - Decision Tree Regressor

4. **Evaluation**
   - Cross-validation
   - GridSearchCV for hyperparameter tuning
   - Final model selection based on performance metrics

## 🤖 Modeling

After cleaning and preprocessing the data, various regression models were trained and evaluated. The final model was selected based on **R² score**, **MAE**, and **cross-validation** results.

### Best Performing Model:
- **Linear Regression with L2 regularization (Ridge)**
- Saved using Pickle (`model.pickle`)

## 📈 Results

- R² Score: ~0.82
- Model performs well for mid-range and high-density location predictions.
- Errors are higher in sparse/less common localities due to fewer data points.



