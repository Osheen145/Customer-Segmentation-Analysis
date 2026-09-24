# Customer Segmentation Analysis

## Project Overview

This project focuses on segmenting customers based on their purchasing behavior using **RFM (Recency, Frequency, Monetary) analysis** and **K-Means clustering**.

The analysis identifies three customer groups:

- **High-Value Customers**
- **Regular Customers**
- **At-Risk Customers**

The results are presented through **interactive Tableau dashboards** to understand customer behavior, product preferences, and geographic distribution.

---

## Project Objectives

- Clean and preprocess retail transaction data.
- Analyze customer purchasing behavior using RFM analysis.
- Apply K-Means clustering for customer segmentation.
- Use silhouette analysis to select the appropriate number of clusters.
- Analyze product preferences across customer segments.
- Analyze customer distribution by country.
- Create interactive Tableau dashboards.
- Generate actionable business recommendations.

---

## Dataset

The project uses the **Online Retail Dataset** from Kaggle.

### Dataset Summary

| Stage | Records / Customers |
|---|---:|
| Original transaction records | 541,909 |
| Cleaned transaction records | 397,884 |
| Unique customers used for analysis | 4,338 |

### Dataset Features

| Column | Description |
|---|---|
| InvoiceNo | Transaction/invoice number |
| StockCode | Product identification code |
| Description | Product description |
| Quantity | Number of items purchased |
| InvoiceDate | Date and time of transaction |
| UnitPrice | Price per item |
| CustomerID | Unique customer identifier |
| Country | Customer's country |

---

## Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Scikit-learn**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook**
- **Tableau**
- **Git & GitHub**

---

## Project Workflow

```text
Raw Dataset
     ↓
Data Cleaning
     ↓
RFM Feature Engineering
     ↓
Feature Scaling
     ↓
K-Means Clustering
     ↓
Silhouette Analysis
     ↓
Customer Segmentation
     ↓
Tableau Visualization
     ↓
Business Insights & Recommendations

---

## RFM Analysis

RFM analysis was used to measure customer purchasing behavior.

### Recency

Number of days since a customer's most recent purchase.

**Lower Recency = More Recent Customer Activity**

### Frequency

Number of purchases/transactions made by a customer.

**Higher Frequency = More Frequent Purchases**

### Monetary

Total amount spent by a customer.

**Higher Monetary Value = Higher Customer Value**

### RFM Summary

| Metric | Mean | Minimum | Maximum |
|---|---:|---:|---:|
| Recency (days) | 92.54 | 1 | 374 |
| Frequency | 4.27 | 1 | 209 |
| Monetary | 2,054.27 | 3.75 | 280,206.02 |

---

## K-Means Clustering

K-Means clustering was applied to the standardized RFM features to group customers with similar purchasing behavior.

Silhouette analysis was used to evaluate different cluster sizes. The final model uses **3 customer segments**.

---

## Customer Segmentation Results

| Segment | Customers | Avg Recency | Avg Frequency | Avg Monetary | Total Revenue |
|---|---:|---:|---:|---:|---:|
| High-Value Customers | 962 | 26.90 | 8.16 | 3,008.21 | 2,893,902.43 |
| Regular Customers | 2,327 | 48.97 | 2.46 | 731.49 | 1,702,173.86 |
| At-Risk Customers | 1,049 | 244.86 | 1.47 | 427.68 | 448,637.74 |

---

## Customer Segment Interpretation

### 1. High-Value Customers

These customers purchase frequently, have purchased recently, and spend significantly more than the other segments.

**Recommended strategies:**

- Loyalty rewards
- Exclusive offers
- Personalized recommendations
- Retention campaigns
- Early access to new products

### 2. Regular Customers

Regular Customers form the largest segment and show moderate purchasing frequency and spending.

**Recommended strategies:**

- Cross-selling
- Upselling
- Product bundles
- Personalized recommendations
- Incentives to increase purchase frequency

### 3. At-Risk Customers

At-Risk Customers have high recency and low purchase frequency, indicating reduced recent engagement.

**Recommended strategies:**

- Win-back campaigns
- Personalized discounts
- Email reminders
- Re-engagement offers
- Recommendations based on previous purchases

---

##Tableau Dashboards

The project contains two interactive Tableau dashboards.

Dashboard 1 — Customer Segmentation Analysis

The dashboard provides:

Total Customers
Total Revenue
Average Customer Value
Customer distribution by segment
Revenue contribution by segment
Customer Frequency vs Spending
Average Recency by Segment
Dashboard 2 — Customer Preferences & Demographics

The dashboard provides:

Top 10 Countries by Customer Count
Top 10 Products by Customer Segment
Customer Segment filter
Country filter
Dashboard Preview
Customer Segmentation Analysis

Customer Preferences & Demographics

The complete Tableau workbook containing both dashboards is available in the Tableau folder.

---

##Key Business Insights

###1. High-Value Customers drive revenue

High-Value Customers represent approximately 22% of the customer base but contribute approximately 57% of total revenue.

###2. High-Value Customers are more active

Their average purchase frequency is 8.16, compared with 2.46 for Regular Customers and 1.47 for At-Risk Customers.

###3. At-Risk Customers show low recent engagement

At-Risk Customers have an average recency of approximately 245 days, compared with approximately 27 days for High-Value Customers.

###4. Regular Customers are the largest segment

Regular Customers account for 2,327 customers, representing roughly 54% of the customer base.

###5. Product preferences can support targeted marketing

The Tableau dashboard allows product purchasing patterns to be explored by customer segment, helping businesses design more relevant and personalized marketing campaigns.

---

## Business Recommendations

| Customer Segment | Recommended Strategy |
|---|---|
| High-Value | Retention, loyalty rewards, exclusive offers |
| Regular | Upselling, cross-selling, bundles |
| At-Risk | Win-back campaigns, discounts, re-engagement |

---

## Repository Structure

```text
Customer-Segmentation-Analysis/
│
├── Dataset/
│   └── Online Retail.xlsx
│
├── Tableau/
│   ├── Customer_Segmentation.twbx
│   ├── customer_segments.csv
│   ├── product_preferences.csv
│   ├── dashboard_1.png
│   └── dashboard_2.png
│
├── Python/
│   └── customer_segmentation.ipynb
│
├── Report/
│   └── Customer_Segmentation_Report.pdf
│
├── .gitignore
└── README.md
```

---

## Conclusion

This project demonstrates an end-to-end customer analytics workflow covering data cleaning, RFM analysis, feature scaling, K-Means clustering, Tableau visualization, and business interpretation.

The segmentation identifies valuable customers, regular customers with growth potential, and customers who may require reactivation. These insights can support targeted marketing, customer retention, personalized recommendations, and revenue growth.

---

## Author 

**Osheen Dongre**


