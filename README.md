# Predicting Late Deliveries in Brazilian E-Commerce: Olist Marketplace Study

## Description
This project explores whether late deliveries on the Brazilian e-commerce site **Olist** can be forecasted at the point of order placement using machine learning. Using the Brazilian E-Commerce Public Dataset (2016-2018), the study analyzes approximately 100,000 orders to identify high-risk deliveries before they occur, enabling proactive operational decisions.

## Key Features
* **Data Integration**: Merges multiple Olist tables (orders, items, customers, sellers, and products) into a unified modeling dataset of ~94,000 orders.
* **Feature Engineering**: Utilizes only "purchase-time" variables to ensure real-world applicability, including price, freight cost, product category, customer/seller locations, and temporal factors (month, day of week).
* **Predictive Modeling**: Compares a **Logistic Regression** baseline with a **Random Forest** classifier to handle the natural class imbalance (7-8% late orders).
* **Performance Analysis**: Evaluates models using Precision, Recall, and F1-scores, highlighting Random Forest's superior ability to detect late-delivery instances.

## Technologies Used
* **Language**: Python
* **Libraries**: pandas, scikit-learn, Matplotlib, Seaborn
* **Environment**: Jupyter Notebooks

## Repository Structure
* `01_data_preparation.ipynb`: Loads raw tables, performs cleaning, and merges data.
* `02_eda_feature_engineering.ipynb`: Conducts exploratory data analysis and generates final modelling features.
* `03_modelling.ipynb`: Trains and evaluates the machine learning models and generates performance reports.
* **Artifacts**: Saved model files (`.joblib`) and evaluation metrics (`.txt`).

## How to Reproduce
To regenerate the results and artifacts, run the notebooks in the following order:
1. **`01_data_preparation.ipynb`**: Prepare the processed dataset.
2. **`02_eda_feature_engineering.ipynb`**: Perform EDA and feature creation.
3. **`03_modelling.ipynb`**: Train models and generate evaluation metrics.
