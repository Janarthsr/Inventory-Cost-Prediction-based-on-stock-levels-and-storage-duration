Name: Janarth S R (AIML) (1CD24AI047)
# Inventory-Cost-Prediction-based-on-stock-levels-and-storage-duration
Predicting Holding Cost using Inventory Cost Dataset
📦 Inventory Management: Holding Cost Prediction
1. TOPIC AND PROBLEM STATEMENT
Topic: Predictive Modeling of Warehouse Inventory Holding Costs. Problem Statement: Excessive inventory leads to high holding costs, while too little stock results in stockouts. This project aims to build a machine learning model to predict Total Holding Costs based on inventory levels and storage rates, allowing businesses to optimize their capital allocation and warehouse efficiency.

2. DATASET DESCRIPTION
Source File: inventory_holding_data.csv

Target Variable: Holding_Cost (The total expense of maintaining stock).

Key Feature Variables:

Average_Inventory_Level: Mean quantity of stock held.

Storage_Cost_Per_Unit: Rate charged per item for storage.

Lead_Time: Days between order placement and receipt.

SKU_Category: Grouping of products based on type or value.

3. DATA MANIPULATION (PREPROCESSING)
To ensure the model identified the correct financial patterns, the following steps were taken:

Handling Nulls: Automated removal of incomplete records to maintain data integrity.

Feature Scaling: Applied StandardScaler to ensure that features with large ranges (Inventory Levels) did not statistically overpower smaller variables (Cost per unit).

Correlation Analysis: Identified the strongest drivers of cost to eliminate redundant "noise" from the model.

4. MODELS EVALUATED
I implemented a variety of regression algorithms to compare performance:

Linear Regression: Tested for a simple direct relationship between stock levels and costs.

Random Forest Regressor: A committee-based ensemble model used to capture non-linear relationships between lead times and storage expenses.

Gradient Boosting (XGBoost/LightGBM): Used to minimize errors in high-cost SKU categories through iterative learning.

5. INTERPRETATION OF RESULTS
Model Accuracy: Unlike the network latency project, this dataset showed a strong logical structure, resulting in a high positive R² score.

Primary Driver: The analysis revealed that Average Inventory Level combined with Storage Cost per Unit were the primary predictors of the total expense.

Business Conclusion: The model provides highly accurate budget forecasts, allowing warehouse managers to predict monthly storage expenses within a very small margin of error.

6. FUTURE SCOPE
Demand Integration: Adding "Sales Forecast" data could turn this from a cost-prediction tool into a "Profit Optimization" tool.

Seasonality Factors: Incorporating time-series data to account for peak holiday seasons where storage costs often spike.
