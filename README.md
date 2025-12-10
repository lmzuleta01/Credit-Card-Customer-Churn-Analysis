# 💳 Credit Card Customer Churn Analysis

![Project Workflow](https://img.shields.io/badge/Workflow-Complete-brightgreen)
![Machine Learning](https://img.shields.io/badge/ML-Random%20Forest-orange)
![Accuracy](https://img.shields.io/badge/Accuracy-95%25-blue)

A comprehensive end-to-end analysis of customer churn for a fictional credit card company, combining **data engineering**, **machine learning**, and **business intelligence visualization**.

## 🎯 Project Overview

This project analyzes customer churn patterns using financial behavior data. The goal is to:
- Understand key financial behaviors that influence churn
- Build a predictive model to identify at-risk customers
- Visualize insights through an interactive dashboard for banks

## 📊 Project Architecture
#### Raw CSV Data → SQL Server (Data Engineering) → Python (Machine Learning) → Power BI (Visualization) → Business Insights


## 🧮 1. Data Engineering (SQL)

### Data Loading & Cleaning
- Imported raw CSV data into SQL Server
- Structured data into normalized tables
- Handled missing values and standardized formatting
- Ensured consistent data types across all tables

### Feature Engineering
Created behavior-based features to quantify customer activity:
- **Transaction Count Change** (Q4 vs Q1)
- **Transaction Amount Change** (Q4 vs Q1)
- **Credit Utilization Ratio**
- **Months Inactive**
- **Customer Lifetime Metrics**
- **Payment Behavior Patterns**

## 🧠 2. Machine Learning (Python)

### Model Development
- **Algorithm**: Random Forest Classifier
- **Class Handling**: `class_weight="balanced"` to address churn rarity
- **Features**: 15+ engineered financial behavior metrics
- **Target**: Churn status (0 = Retained, 1 = Churned)

### Model Performance
| Metric | Value |
|--------|-------|
| **Overall Accuracy** | 94.8% |
| **Precision (Churn)** | 0.82 |
| **Recall (Churn)** | 0.87 |
| **F1-Score (Churn)** | 0.84 |
### Confusion Matrix 
|  |Predicted Stay | Predicted Churn |
|--------|--------|-------|
| **Actual Stay**| 1638 |  63 |
| **Actual Churn**| 42  | 283 |


### Outputs
- Churn probability scores for each customer
- Feature importance analysis
- Results exported back to SQL for visualization

## 📊 3. Dashboard (Power BI)

### Dashboard Components
- **Churn Distribution**: By demographic segments (age, education, income)
- **Financial Behavior**: Utilization patterns, transaction trends
- **Risk Analysis**: Probability scores across customer segments
- **Time Series**: Behavioral changes leading to churn

### Key Insights Visualized
1. **High-Risk Segments**: Identified demographics with highest churn rates
2. **Behavioral Patterns**: Financial habits preceding churn events
3. **Early Warning Signals**: Key metrics indicating churn risk
4. **Customer Segmentation**: Group-based risk profiling

## 🚀 Key Features

- **End-to-End Pipeline**: Complete workflow from raw data to business insights
- **Reproducible Workflow**: Modular code structure for easy replication
- **Scalable Architecture**: Can handle larger datasets with minimal changes
- **Actionable Insights**: Business-focused metrics and visualizations
- **High Accuracy**: 95% prediction accuracy with balanced metrics



