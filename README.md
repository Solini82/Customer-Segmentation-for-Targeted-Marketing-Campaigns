# Customer Segmentation for Targeted Marketing Campaigns

## Overview
This project segments customers based on their purchasing behavior using **RFM analysis** and **machine learning techniques**. The insights are used to develop targeted marketing strategies to improve customer engagement, retention, and revenue.

---

## Table of Contents
1. [Project Overview](#overview)
2. [Dataset](#dataset)
3. [Methodology](#methodology)
4. [Key Insights](#key-insights)
5. [Installation](#installation)

---

## Dataset
The dataset used is the **Online Retail Dataset**, which contains transactional data for an online retail store. It includes the following columns:
- `InvoiceNo`: Unique identifier for each transaction.
- `StockCode`: Unique identifier for each product.
- `Description`: Description of the product.
- `Quantity`: Number of units purchased.
- `InvoiceDate`: Date and time of the transaction.
- `UnitPrice`: Price per unit of the product.
- `CustomerID`: Unique identifier for each customer.
- `Country`: Country where the transaction occurred.

**Dataset Source:** [Online Retail Dataset](https://archive.ics.uci.edu/ml/datasets/Online+Retail)

---

## Methodology
1. **Data Cleaning:**
   - Handled missing values and removed canceled orders.
   - Created new features like `TotalSpend`.

2. **Exploratory Data Analysis (EDA):**
   - Analyzed customer distribution by country, top products, and total spend.

3. **Customer Segmentation:**
   - Used **RFM analysis** to calculate Recency, Frequency, and Monetary values.
   - Applied **K-Means clustering** to group customers into segments.

4. **Predictive Modeling:**
   - Built a **Random Forest model** to predict customer churn.

5. **Customer Lifetime Value (CLV):**
   - Calculated CLV for each customer segment.

---

## Key Insights
1. **Customer Segments:**
   - Identified key segments such as **Champions**, **Loyal Customers**, **Potential Loyalists**, and **At Risk**.
   - High-value segments (e.g., **551 Segment**) contribute significantly to revenue.

2. **Churn Prediction:**
   - The Random Forest model achieved **perfect accuracy** (1.00) in predicting churn.
   - **Recency** and **Frequency** are the most important factors in predicting churn.

3. **Customer Lifetime Value (CLV):**
   - The **551 Segment** has the highest CLV (**$1,765,910**), making it the most valuable customer group.

4. **Actionable Recommendations:**
   - Proposed targeted marketing strategies for each segment to improve engagement and retention.

---

## Installation
To run this project, you’ll need the following Python libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn plotly
