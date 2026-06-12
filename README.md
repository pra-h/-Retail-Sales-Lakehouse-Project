# 🏪 Retail Sales Lakehouse | Databricks, PySpark, Delta Lake, ML

[![Databricks](https://img.shields.io/badge/Databricks-Community%20Edition-FF3621?style=flat&logo=databricks&logoColor=white)](https://community.cloud.databricks.com)
[![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python&logoColor=white)](https://www.python.org)
[![Spark](https://img.shields.io/badge/Apache%20Spark-3.x-E25A1C?style=flat&logo=apachespark&logoColor=white)](https://spark.apache.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📊 Overview

An **end-to-end data engineering project** implementing the industry-standard **Medallion Architecture (Bronze → Silver → Gold)** on Databricks. Processes 541K+ retail transactions to deliver business insights through SQL analytics, ML models, and interactive dashboards.


---

## 🎯 Key Features

### Data Engineering
- **ETL Pipeline:** Bronze → Silver → Gold using PySpark
- **Data Quality:** 7 cleaning steps → 28% bad data removed
- **Delta Lake:** ACID transactions, versioning, schema enforcement
- **Feature Engineering:** TotalAmount, Year, Month, Day extraction

### SQL Analytics (10 Queries)
1. Top 10 Products by Revenue
2. Monthly Revenue Trends
3. Top 10 Countries
4. Top 10 Customers
5. Best Sales Days
6. Customer Segmentation by Spending
7. Product Category Performance
8. Month-over-Month Growth
9. Revenue per Customer by Country
10. KPI Summary Dashboard

### Machine Learning
| Model | Algorithm | Result |
|-------|-----------|--------|
| **Sales Forecasting** | Linear Regression | R² = 0.82 |
| **Customer Segmentation** | K-Means (k=4) | 4 segments found |

### Dashboard (7 Charts)
- 📈 Revenue Trend Line Chart
- 🏆 Top 10 Products Bar Chart
- 🌍 Country Sales Pie Chart
- 👥 Customer Segments Analysis
- 📅 Best Revenue Days
- 🎯 KPI Summary Cards
- 📈 Growth Rate Combo Chart

---

## 📊 Key Metrics

| KPI | Value |
|-----|-------|
| 💰 Total Revenue | **$8.9 Million** |
| 📊 Avg Monthly Revenue | **$743,000** |
| 🛒 Total Orders | **22,190** |
| 📦 Unique Products | **4,070** |
| 👥 Total Customers | **4,372** |
| 🌍 Countries Served | **38** |
| 💵 Avg Order Value | **$402** |

---

## 🛠️ Tech Stack

| Category | Technology |
|----------|------------|
| **Platform** | Databricks Community Edition |
| **Processing** | Apache Spark, PySpark |
| **Storage** | Delta Lake |
| **Languages** | Python, Spark SQL |
| **ML** | Scikit-learn, Pandas, NumPy |
| **Visualization** | Matplotlib |
| **Dataset** | UCI Online Retail Dataset |

---

## 🚀 How to Run

### Prerequisites
- [Databricks Community Edition](https://community.cloud.databricks.com) (Free)
- [Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)

### Steps

```bash
# 1. Create free Databricks account
# Go to: https://community.cloud.databricks.com

# 2. Upload dataset
# Data → Create Table → Upload File → Select CSV

# 3. Run notebooks in order
01_data_ingestion_bronze    → Creates Bronze table
02_data_cleaning_silver     → Creates Silver table
03_business_tables_gold     → Creates 5 Gold tables
04_sql_analytics           → Run SQL queries
05_ml_forecasting          → Train ML models
06_dashboard               → View dashboards
