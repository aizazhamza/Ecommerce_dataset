# 🛒 E-Commerce Data Analysis & Sales Forecasting

A complete **Data Science and Machine Learning project** based on a large-scale e-commerce dataset containing **1M+ records**. The project focuses on data cleaning, exploratory data analysis (EDA), feature engineering, sales analysis, and machine learning-based sales forecasting.

## 📌 Project Overview

This project analyzes historical e-commerce transaction data to identify important trends, patterns, customer behavior, and sales performance.

The main objective is to transform raw e-commerce data into meaningful business insights and develop a machine learning model capable of forecasting sales using historical and engineered features.

## 🎯 Objectives

* Understand the structure and characteristics of a 1M+ record dataset
* Clean and preprocess raw e-commerce data
* Analyze missing values and data quality
* Perform exploratory data analysis (EDA)
* Identify sales trends and seasonal patterns
* Analyze customer and order behavior
* Perform feature engineering
* Create lag and rolling-window features
* Develop a machine learning model for sales forecasting
* Evaluate model performance
* Generate actionable business insights

## 📊 Dataset

**Dataset:** Global E-Commerce Dataset
**Records:** 1M+
**Time Period:** 2024–2026

The dataset contains information related to:

* Orders
* Customers
* Products
* Pricing
* Quantity
* Revenue / sales
* Profit
* Payment methods and status
* Delivery status
* Customer segments
* Discounts and coupons
* Marketing campaigns
* Traffic sources
* Customer feedback
* Order dates and time-related information

> The raw large CSV dataset is not included in this GitHub repository because of GitHub's file-size limitations.

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**
* **Jupyter Notebook**
* **Git & GitHub**
* **SQL**

## 🔄 Project Workflow

```text
Raw Dataset
     ↓
Data Understanding
     ↓
Data Cleaning
     ↓
Missing Value Handling
     ↓
Exploratory Data Analysis
     ↓
Feature Engineering
     ↓
Time-Series Features
     ↓
Train/Test Split
     ↓
Machine Learning Model
     ↓
Model Evaluation
     ↓
Sales Forecasting
     ↓
Business Recommendations
```

## 🧹 Data Cleaning

The preprocessing stage includes:

* Checking dataset dimensions
* Checking data types
* Identifying duplicate records
* Detecting missing values
* Handling missing values
* Converting date columns
* Encoding categorical variables
* Removing unnecessary columns
* Checking outliers and unusual values

## 📈 Exploratory Data Analysis

The analysis explores:

* Sales trends over time
* Monthly and quarterly sales
* Customer segments
* Order status
* Payment status
* Product and category performance
* Profit and revenue relationships
* Customer behavior
* Promotional effects
* Seasonal patterns

### Quarterly Sales

The analysis showed relatively balanced quarterly sales, with **Q3 having the highest total sales**, followed by Q4, Q2, and Q1.

## ⚙️ Feature Engineering

Several time-based and forecasting features were created from the order date, including:

* Year
* Month
* Quarter
* Day
* Day of week
* Weekend indicator
* Lag features
* Rolling-window features
* Promotional/seasonal indicators

### Forecasting Features

Important forecasting features include:

```text
lag_1
lag_7
lag_30
rolling_7
rolling_30
```

These features capture recent sales behavior and historical trends.

## 🤖 Machine Learning

A **Random Forest Regressor** was developed for sales forecasting.

The dataset was divided into training and testing sets:

```text
X_train: 800,098 rows × 62 features
X_test:  200,025 rows × 62 features

y_train: 800,098 rows
y_test:  200,025 rows
```

### Feature Importance

The most important forecasting features included:

| Feature    | Importance |
| ---------- | ---------: |
| rolling_7  |    ~17.77% |
| rolling_30 |    ~17.22% |
| lag_1      |    ~17.19% |
| lag_30     |    ~16.88% |
| lag_7      |    ~16.78% |

The results indicate that **recent historical sales behavior is highly influential for forecasting future sales**.

## 📊 Key Insights

Some important findings from the analysis include:

* Sales remained relatively stable across quarters.
* Recent historical sales strongly influenced forecasting.
* Rolling-window features captured short-term and medium-term sales patterns.
* Customer and transaction characteristics provide useful information for predicting sales.
* Feature engineering significantly improves the usefulness of raw transactional data for machine learning.

## 💡 Business Recommendations

Based on the analysis, businesses can:

1. Monitor recent sales trends to improve demand forecasting.
2. Use rolling sales statistics for inventory planning.
3. Analyze customer segments to develop targeted marketing strategies.
4. Monitor promotional campaigns and their effect on sales.
5. Use forecasting models to support inventory and resource planning.
6. Continuously update forecasting features as new transactions become available.

## 📁 Repository Structure

```text
Ecommerce_dataset/
│
├── data_set/
│   └── README.md
│
├── ecommerce_2.ipynb
│
├── .gitignore
│
└── README.md
```

> The original large dataset is intentionally excluded from the repository.

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/aizazhamza/Ecommerce_dataset.git
cd Ecommerce_dataset
```

### 2. Create a Python environment

```bash
python -m venv venv
```

### 3. Activate the environment

**Windows:**

```bash
venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### 5. Open the notebook

```bash
jupyter notebook ecommerce_2.ipynb
```

## 📌 Project Status

**Completed**

The project currently includes:

* Data preprocessing
* Exploratory data analysis
* Feature engineering
* Time-based analysis
* Sales forecasting features
* Machine learning model development
* Feature importance analysis
* Business recommendations

## 👨‍💻 Author

**Aizaz Hamza**

Computer Science Graduate | AI & Data Science Enthusiast

### Skills Demonstrated

`Python` `Pandas` `NumPy` `Matplotlib` `Seaborn` `Scikit-learn` `SQL` `EDA` `Feature Engineering` `Machine Learning` `Data Visualization` `Sales Forecasting`

---

⭐ If you find this project useful, consider giving the repository a star.
