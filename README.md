# 🛍️ Retail Sales & Customer Segmentation Analysis

An end-to-end data analytics project analyzing UK-based online retail transaction data — covering data cleaning, exploratory analysis, RFM-based customer segmentation with K-Means clustering, and an interactive Power BI dashboard.

## 📌 Project Overview

This project analyzes ~541K retail transactions to uncover sales trends, top-performing products/markets, and distinct customer segments — turning raw transaction logs into actionable business insights.

## 🔧 Tools & Technologies
- **Python** (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- **Google Colab** (development environment)
- **Power BI** (interactive dashboard)
- **Machine Learning**: K-Means Clustering for customer segmentation

## 🗂️ Dataset
[Online Retail Dataset](https://www.kaggle.com/datasets/vijayuv/onlineretail) — 541,909 transactions from a UK-based online retailer (Dec 2010–Dec 2011).

## 🧹 Data Cleaning
- Removed ~135K rows with missing CustomerIDs
- Removed 5,225 duplicate transactions
- Filtered out returns/cancellations (negative quantities/prices)
- Final cleaned dataset: **401,604 transactions**

## 📊 Key Insights

### 1. Seasonal Sales Spike
Revenue peaked sharply in **November** (₹11.56L), nearly double the mid-year average — strongly suggesting holiday/pre-Christmas shopping behavior.

### 2. Market Concentration
The **UK accounts for the vast majority of revenue**, with all other countries combined contributing a small fraction — highlighting the business's near-total dependence on its home market.

### 3. Customer Segmentation (RFM + K-Means)
Using Recency, Frequency, and Monetary analysis, customers were grouped into 4 segments:

| Segment | Description | % of Total Revenue |
|---|---|---|
| VIP / Champions | Extremely frequent, high-spend buyers (likely wholesale) | 18.6% |
| Loyal Customers | Frequent, recent, healthy spend | 29.1% |
| Regular/Casual | Bulk of customer base, moderate spend | 46.5% |
| At Risk/Churned | Inactive 8+ months, low engagement | 5.7% |

**Key finding:** VIP + Loyal segments make up a minority of customers by count but generate nearly **48% of total revenue** — a classic Pareto (80/20) pattern, while the At-Risk segment represents a clear re-engagement opportunity.

## 📈 Dashboard

Built an interactive 4-page Power BI dashboard covering:
1. Revenue by Customer Segment
2. Monthly Sales Trend
3. Top 10 Countries by Revenue
4. Top 10 Best-Selling Products

*(See screenshots in `/visuals`)*

## 📁 Project Structure
```
retail-sales-insights/
├── data/
│   ├── OnlineRetail.csv
│   ├── cleaned_retail.csv
│   └── rfm_segments.csv
├── notebooks/
│   └── retail_analysis.ipynb
├── visuals/
│   ├── monthly_sales_trend.png
│   ├── top_products.png
│   ├── top_countries.png
│   ├── sales_by_day.png
│   ├── elbow_method.png
│   └── powerbi_dashboard_page1.png
├── dashboard/
│   └── retail_dashboard.pbix
└── README.md
```

## 🚀 How to Run
1. Clone this repo
2. Open `notebooks/retail_analysis.ipynb` in Google Colab or Jupyter
3. Open `dashboard/retail_dashboard.pbix` in Power BI Desktop to explore the interactive dashboard

## 👤 Author
Aarya — B.Tech Computer Engineering (AI Specialization), SAKEC Mumbai

---
⭐ If you found this project useful, consider giving it a star!
