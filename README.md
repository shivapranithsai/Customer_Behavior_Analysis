🛍️ Customer Shopping Behavior & Segmentation Analysis

Python
MySQL
Power BI

An end-to-end data analytics project examining customer purchasing habits, demographic breakdowns, subscription impact, and loyalty segmentation across 3,900 customer transactions.

📌 Project Overview

This project provides a full analytics pipeline to help retailers understand customer purchasing patterns and optimize sales strategies:

Python (Pandas & SQLAlchemy): Data cleaning, missing value imputation, and feature engineering.
MySQL: Relational database modeling, customer segmentation, and business queries.
Power BI: Interactive executive dashboard tracking revenue trends, and demographic behavior.

⚙️ Workflow & Key Highlights
1. Data Cleaning & Feature Engineering (Python)
Imputed missing Review Rating values using category-level medians.
Standardized column names to snake_case.
Engineered new features:
age_group: Categorized into 4 demographic cohorts (young_adult, adult, middle_aged, senior).
purchase_frequency_days: Standardized frequencies into numeric day intervals.
Removed collinear redundant features (promo_code_used).
Streamed cleaned data directly into MySQL using SQLAlchemy.
2. SQL Business Analysis (MySQL)

The customer_behaviour_analysis_queries.sql script answers 10 key business questions, including:

Revenue by Demographics: Revenue contributions across age groups and gender.
Customer Segmentation: Categorized into New (1 purchase), Returning (2–10), and Loyal (>10 purchases).
Subscription Financial Impact: Spend and revenue comparison between subscribers and non-subscribers.
Top Products per Category: Ranked using ROW_NUMBER() window functions and CTEs.
Promotions & Fulfillment: High-spending discount users and spend comparison across shipping types.
3. Interactive Dashboard (Power BI)
KPI Metrics: Total Revenue ($233K), Total Orders (3.9K), Average Spend ($59.76), and Average Rating (3.75).
Visuals: Sales by category, demographic distribution, shipping preferences, and subscription status.
Filters: Interactive slicers for dynamic drill-downs by category, season, and gender.
💡 Key Findings
High Customer Loyalty: ~80% of customers have made more than 10 purchases, representing a solid repeat-buyer base.
Top Product Categories: Clothing ($104K+) and Accessories ($74K+) generate the largest share of total revenue.
Discount Sensitivity: Products like Hats, Sneakers, and Coats had the highest discount rates (~50%).
Subscription Potential: High-frequency repeat buyers (>5 purchases) are prime candidates for subscription upsells.
🚀 How to Run

Clone the Repo:

bash
git clone https://github.com/shivapranithsai/Customer_behavior_analysis.git
cd Customer_behavior_analysis

Run Python Pipeline:

bash
pip install pandas sqlalchemy pymysql jupyter
jupyter notebook "Customer_behaviour (2).ipynb"

Run SQL Queries: Open and execute customer_behaviour_analysis_queries.sql in MySQL Workbench or your favorite SQL client.

View Power BI Dashboard: Open Customer_Behavior_Dashboard.pbix in Power BI Desktop
.

🛠️ Tech Stack
Languages & Libraries: Python (Pandas, SQLAlchemy, PyMySQL), SQL
Database: MySQL 8.0+
BI & Visualization: Microsoft Power BI Desktop


👤 Author
GitHub: @shivapranithsai

(Feel free to star ⭐ this repository if you found it useful!)
