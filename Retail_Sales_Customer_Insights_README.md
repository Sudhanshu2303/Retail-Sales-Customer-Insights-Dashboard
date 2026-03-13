
# Retail Sales & Customer Insights Dashboard

## Project Overview
This project focuses on analyzing retail transaction data to identify revenue drivers, customer purchasing behavior, and product performance trends. The objective is to transform raw transactional data into actionable business insights through data cleaning, exploratory analysis, and an interactive Power BI dashboard.

The project demonstrates practical data analytics skills including data preprocessing, SQL querying, exploratory data analysis (EDA), and data visualization to support data-driven decision-making in retail businesses.

---

# Business Problem
Retail companies often collect large volumes of transactional data but struggle to extract meaningful insights that can improve business performance. Without structured analysis, businesses face challenges such as:

- Identifying high-value customers
- Detecting loss-making products
- Understanding regional sales performance
- Tracking key performance indicators (KPIs)
- Recognizing seasonal sales patterns

This project aims to solve these challenges by building a data analytics pipeline and an interactive dashboard that enables stakeholders to monitor business performance and make strategic decisions.

---

# Dataset Information

Dataset Type: Retail Sales Transactions

Dataset Size
- Records: 9,994 transactions
- Features: 21 columns

Example Features
- Order ID
- Order Date
- Customer ID
- Customer Segment
- Region
- Product Category
- Product Subcategory
- Sales
- Quantity
- Discount
- Profit

The dataset represents transactional retail data commonly used for sales performance analysis and business intelligence applications.

---

# Project Workflow

The project follows a structured data analytics lifecycle.

## 1. Data Collection
The dataset was obtained from a publicly available retail dataset commonly used for business analytics practice.

---

## 2. Data Cleaning and Preprocessing

Data preprocessing was performed using Python (Pandas, NumPy).

Tasks performed:

- Handling missing values
- Removing duplicate records
- Converting date columns into proper datetime format
- Standardizing categorical values
- Checking data consistency across features

Clean data ensures reliable and accurate analysis results.

---

## 3. Exploratory Data Analysis (EDA)

Exploratory analysis was performed to identify patterns and insights in the dataset.

EDA tasks included:

- Sales distribution analysis
- Profitability analysis
- Regional performance comparison
- Category-wise sales analysis
- Monthly trend analysis

Libraries used:
- Pandas
- Matplotlib
- Seaborn

---

# SQL Data Analysis

SQL was used to perform business-focused queries such as:

## Top Selling Product Categories
```sql
SELECT Category, SUM(Sales)
FROM sales_data
GROUP BY Category
ORDER BY SUM(Sales) DESC;
```

## Regional Sales Performance
```sql
SELECT Region, SUM(Sales)
FROM sales_data
GROUP BY Region;
```

## Top Customers by Revenue
```sql
SELECT Customer_ID, SUM(Sales)
FROM sales_data
GROUP BY Customer_ID
ORDER BY SUM(Sales) DESC
LIMIT 10;
```

SQL helped perform efficient data aggregation and business performance analysis.

---

# Power BI Dashboard

An interactive Power BI dashboard was created to visualize the key insights.

## Key KPIs

- Total Revenue
- Profit Margin %
- Average Order Value (AOV)
- Year-over-Year Growth

---

## Dashboard Features

### Sales Overview
Displays total revenue and sales trends across different regions and time periods.

### Customer Insights
Identifies high-value customers and purchasing patterns.

### Product Performance
Shows top-performing product categories and loss-making products.

### Regional Sales Analysis
Compares revenue across multiple regions.

### Monthly Sales Trends
Tracks seasonal demand fluctuations.

---

## Interactive Features

The dashboard allows users to interact with the data using:

- Dynamic filters
- Region slicers
- Category filters
- Date filters
- Drill-down capabilities

These features allow stakeholders to explore data from multiple perspectives.

---

# Key Insights

- Top 20% customers generated approximately 68% of total revenue (Pareto principle).
- Certain product categories showed negative profit margins (~12%), indicating pricing or cost issues.
- Significant seasonal demand fluctuations (~35%) were observed across regions.
- Regional sales performance varied significantly, highlighting potential expansion opportunities.

---

# Tools and Technologies

| Tool | Purpose |
|-----|-----|
| Python | Data cleaning and preprocessing |
| Pandas | Data manipulation |
| NumPy | Numerical computations |
| SQL | Business data analysis |
| Power BI | Interactive dashboard visualization |
| Excel | Initial data exploration |

---

# Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- SQL Data Analysis
- Data Visualization
- Business Intelligence
- KPI Dashboard Development
- Customer Segmentation Analysis

---

# Project Structure

```
Retail-Sales-Dashboard
│
├── dataset
│   └── retail_sales.csv
│
├── notebooks
│   └── data_cleaning_analysis.ipynb
│
├── sql_queries
│   └── business_queries.sql
│
├── dashboard
│   └── retail_dashboard.pbix
│
└── README.md
```

---

# Future Improvements

- Sales forecasting using machine learning
- Customer lifetime value prediction
- Product demand forecasting
- Automated data pipeline development
- Dashboard deployment for real-time updates

---

# Conclusion

This project demonstrates how raw retail data can be transformed into meaningful business insights using data analytics tools. By combining Python, SQL, and Power BI, the project provides a comprehensive framework for analyzing sales performance and supporting data-driven business strategies.
