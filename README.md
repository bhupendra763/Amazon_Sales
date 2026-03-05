# Amazon Sales Revenue Prediction & Analysis

A complete Data Analysis and Machine Learning project that analyzes Amazon sales data and predicts total revenue using multiple regression models.

This project demonstrates a full data science workflow including data cleaning, exploratory data analysis (EDA), feature engineering, machine learning model training, and model evaluation.

---

## Project Overview

The goal of this project is to analyze Amazon sales data and build predictive models that estimate **total revenue** based on product attributes, sales performance, and customer behavior.

The project includes:

- Data cleaning and preprocessing
- Data quality assessment
- Exploratory data analysis (EDA)
- Feature engineering
- Machine learning model training
- Model comparison using multiple algorithms

---

## Dataset Features

The dataset contains product sales information such as:

| Feature | Description |
|------|------|
| price | Product price |
| discount_percent | Discount offered on product |
| quantity_sold | Number of units sold |
| rating | Average customer rating |
| review_count | Total number of reviews |
| product_category | Category of product |
| customer_region | Region of customer |
| payment_method | Payment method used |
| month | Month of sale |
| quarter | Sales quarter |
| total_revenue | Target variable |

---

## Project Workflow

### 1. Data Loading
The dataset is loaded using pandas and initial inspection is performed.

### 2. Data Quality Assessment
Data is checked for:

- Missing values
- Data types
- Duplicate records

Duplicates are removed to ensure clean training data.

### 3. Exploratory Data Analysis (EDA)

Visualizations are created to analyze:

- Product category performance
- Revenue distribution
- Ratings vs revenue
- Sales trends

Libraries used:

- Matplotlib
- Seaborn

### 4. Feature Engineering

Categorical features are converted into numerical format using **One-Hot Encoding**.

Example categorical columns:

- product_category
- customer_region
- payment_method

### 5. Train-Test Split

The dataset is split into:

- **80% training data**
- **20% testing data**

This helps evaluate model performance on unseen data.

### 6. Machine Learning Models

The following regression models are trained and compared:

1. Ridge Regression
2. Random Forest Regressor
3. XGBoost Regressor (or Gradient Boosting if XGBoost is unavailable)

### 7. Model Evaluation

Models are evaluated using:

- MAE (Mean Absolute Error)
- RMSE (Root Mean Squared Error)
- R² Score
- Cross Validation Score

The best-performing model is selected based on **highest R² score and lowest error values**.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost

---
