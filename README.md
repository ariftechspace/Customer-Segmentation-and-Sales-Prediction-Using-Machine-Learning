# Retail Sales Intelligence: Customer Segmentation and Sales Prediction Using Machine Learning

## Project Overview

This project is an end to end data science project that analyzes retail sales data using Python and machine learning.

The project focuses on understanding customer purchasing behavior, analyzing sales trends, segmenting customers, and predicting sales. It demonstrates the complete data science workflow from data cleaning to model building and evaluation.

This project was developed as part of my data analytics portfolio.

---

<table align="center">
<tr>
<td align="center">
<img src="figures/monthly_sales_trend.png" width="420"><br>
<b>Monthly Sales Trend</b>
</td>

<td align="center">
<img src="figures/top_categories.png" width="420"><br>
<b>Top Categories</b>
</td>
</tr>

<tr>
<td align="center">
<img src="figures/top_products.png" width="420"><br>
<b>Top Products</b>
</td>

<td align="center">
<img src="figures/top_customers.png" width="420"><br>
<b>Top Customers</b>
</td>
</tr>
</table>


# Business Problem

Retail businesses need to understand customer behavior and sales patterns to make better business decisions.

The main objectives of this project are to:

* Analyze retail sales data
* Identify customer purchasing patterns
* Segment customers into different groups
* Build machine learning models to predict sales
* Generate business insights from the data

---

# Dataset

Dataset: Retail Store Sales Transactions

The dataset contains more than 131,706 retail transactions with information such as:

* Date
* Customer ID
* Transaction ID
* Product Category
* Product (SKU)
* Quantity
* Sales Amount

---

# Tools and Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* Scikit-learn
* Google Colab
* KaggleHub

---

# Project Workflow

1. Data Loading
2. Data Understanding
3. Data Preparation and Inspection
4. Exploratory Data Analysis
5. Feature Engineering
6. Customer Segmentation using K-Means
7. Sales Prediction using Regression Models
8. Model Evaluation
9. Business Insights
10. Conclusion

---

# Machine Learning Models

## Model 1: Customer Segmentation

Algorithm:

* K-Means Clustering

Purpose:

Group customers based on their purchasing behavior.

---

## Model 2: Sales Prediction

Algorithms:

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor

Evaluation Metrics:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

---

# Results

## Customer segments (K-Means, silhouette score 0.58)

| Segment | Avg total spend | Avg purchases | Avg tenure (days) |
|---|---|---|---|
| Loyal high-value | 752.76 | 19.5 | 245 |
| Regular mid-value | 123.45 | 5.5 | 178 |
| Infrequent big-basket | 212.55 | 1.6 | 25 |
| New low-spend | 27.35 | 1.5 | 14 |

## Sales prediction (20% test set)

| Model | MAE | RMSE | R² |
|---|---|---|---|
| Gradient Boosting | 7.19 | 15.59 | 0.333 |
| Linear Regression | 6.67 | 15.98 | 0.299 |
| Random Forest | 7.63 | 16.26 | 0.275 |

# Key Findings

- Four customer groups with very different value: the loyal group spends about 28 times more than the new low-spend group (752.76 vs 27.35).
- Gradient Boosting scored best on R² and RMSE; Linear Regression had the lowest MAE.
- The models explain about a third of the variation in sales amount, so they are a baseline.

# Limitations

Predictions are made per line item, which is hard to forecast. 
Future work: more features, or predicting monthly sales per category.
