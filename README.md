# Customer Segmentation Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

![Dashboard](images/Mini%20Analytics%20Dashboard%20Layout.png)

## Project Overview

This project performs **customer segmentation using RFM (Recency, Frequency, Monetary) analysis** to understand customer purchasing behavior and identify valuable customer groups.

Using clustering techniques, customers are grouped into segments based on their purchasing patterns. These insights help businesses design targeted marketing strategies and improve customer retention.

Customer segments were identified using **K-Means clustering** after scaling the RFM features.

---

# Business Problem

Businesses often have thousands of customers but limited marketing resources.

Key questions include:

- Who are the most valuable customers?
- Which customers are at risk of churning?
- How can marketing efforts be targeted effectively?

Customer segmentation helps answer these questions by grouping customers with similar behaviors.

---

# Project Objectives

The main objectives of this project are:

- Understand customer purchasing behavior
- Identify high-value customers
- Segment customers into meaningful groups
- Generate insights for marketing and business strategy
- Visualize customer behavior patterns

---

# Dataset

The dataset contains transactional data including:

- CustomerID
- InvoiceDate
- InvoiceNo
- Quantity
- UnitPrice

From these variables, the **RFM metrics** were calculated:

| Metric | Description |
|------|-------------|
| Recency | How recently a customer made a purchase |
| Frequency | How often a customer purchases |
| Monetary | Total amount spent by the customer |

---

# Methodology

The project follows a typical **data science workflow**:

### 1. Data Cleaning
- Removed missing values
- Filtered invalid transactions
- Ensured consistent data formatting

### 2. Feature Engineering
RFM metrics were calculated for each customer:

- Recency
- Frequency
- Monetary

### 3. Feature Scaling

Before clustering, features were standardized using  
**StandardScaler** from the :contentReference[oaicite:1]{index=1} algorithm.

### 4. Customer Segmentation

Customers were segmented using  
**K-Means Clustering** from :contentReference[oaicite:2]{index=2}.

The optimal number of clusters was determined using the **Elbow Method**.

### 5. Data Visualization

Multiple visualizations were created to explore customer behavior and interpret the clusters.

---

# Visualizations

## RFM Correlation Heatmap
![RFM Heatmap](images/rfm%20correlation%20heatmap.png)

This heatmap shows the relationship between Recency, Frequency, and Monetary values.

---

## Revenue Contribution by Segment
![Revenue Segment](images/revenue%20contribution%20by%20segment.png)

Shows which customer segments contribute the most revenue.

---

## Revenue Contribution by Cluster
![Revenue Cluster](images/revenue%20contribution%20by%20customer%20cluster.png)

Helps identify which clusters represent the most valuable customers.

---

## Frequency vs Monetary Distribution
![Frequency vs Monetary](images/frequency%20vs%20monetary.png)

Visualizes how frequently customers purchase relative to how much they spend.

---

## Customer Frequency Distribution
![Frequency Distribution](images/frequency%20distribution.png)

Shows how often customers make purchases.

---

## Customer Monetary Distribution
![Monetary Distribution](images/monetary%20distribution.png)

Displays the distribution of customer spending.

---

## Log Transformed Monetary Distribution
![Log Monetary](images/log%20transformed%20monetary%20distribution.png)

Log transformation was used to better understand the spending distribution.

---

## Customer Recency Distribution
![Recency](images/recency%20distribution.png)

Shows how recently customers made purchases.

---

## Elbow Method (Optimal Clusters)
![Elbow](images/elbow%20method.png)

Used to determine the optimal number of clusters for K-Means.

---

## Mini Analytics Dashboard
![Dashboard](images/Mini%20Analytics%20Dashboard%20Layout.png)

A dashboard summarizing key customer segmentation insights.

---

# Key Insights

From the segmentation analysis:

- **VIP customers contribute the largest share of revenue**
- **Loyal customers purchase frequently but spend slightly less per order**
- **At-risk customers have not purchased recently**
- **Low-value customers purchase rarely and spend less**

These insights can help businesses optimize marketing strategies.

---

# Business Recommendations

### VIP Customers
- Provide loyalty rewards
- Offer exclusive promotions
- Maintain strong engagement

### Loyal Customers
- Upsell premium products
- Cross-sell complementary products

### At-Risk Customers
- Run re-engagement campaigns
- Offer targeted discounts

### Low-Value Customers
- Use automated marketing strategies
- Encourage repeat purchases

---

# Tools & Technologies

The following tools were used in this project:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

# Author

**Rafid Musyaffa**

LinkedIn:  
www.linkedin.com/in/rafid-musyaffa-a75079312

GitHub Repository:  
https://github.com/Rafidmusyaffa/customer-segmentation-analysis

Dataset Source:  
https://share.google/NGKUF6mVQXxZAUGLA

---

# Conclusion

Customer segmentation using RFM analysis provides valuable insights into customer behavior. By applying machine learning techniques such as K-Means clustering, businesses can identify high-value customers and design more effective marketing strategies.

This project demonstrates how data science techniques can be used to transform raw transactional data into actionable business insights.