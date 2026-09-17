# Retail Sales Exploratory Data Analysis

## 📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on a retail sales dataset to understand sales trends, customer demographics, product performance, category-level revenue, profitability, and relationships between numerical variables.

The analysis was completed as part of the Oasis Infobyte Data Analytics Internship.

---

## 🎯 Objectives

- Inspect and understand the retail sales dataset.
- Identify missing values and duplicate records.
- Clean and prepare data for analysis.
- Analyze monthly and quarterly sales trends.
- Understand customer demographics based on age and gender.
- Identify the top 10 best-selling products.
- Analyze revenue by product category.
- Study correlations between numerical variables.
- Compare profit margins across product categories.
- Generate actionable business recommendations.

---

## 📊 Dataset

The dataset contains retail transaction information including:

- Order details
- Customer information
- Product categories and products
- Quantity and pricing
- Discounts
- Sales amount
- Profit
- Shipping cost
- Customer satisfaction
- Order status and return information

The dataset contains **4,310 records and 21 columns**.

---

## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- VS Code

---

## 🔍 Project Workflow

### 1. Data Inspection

The dataset was inspected using:

- Shape
- Data types
- Missing value analysis
- Duplicate detection
- Descriptive statistics

### 2. Data Cleaning

The following data preparation steps were performed:

- Converted order dates into a consistent datetime format.
- Identified and handled invalid age values.
- Standardized gender categories.
- Created age groups for demographic analysis.
- Created year, month, month name, and quarter features.
- Identified duplicate records.

### 3. Sales Trend Analysis

Monthly and quarterly sales trends were visualized to understand changes in sales performance over time.

### 4. Customer Demographics

Customer distribution was analyzed using:

- Age groups
- Gender
- Gender-wise sales

### 5. Product Analysis

The top 10 products by quantity sold were identified to understand high-volume products.

### 6. Category Analysis

Revenue was compared across product categories.

### 7. Correlation Analysis

A correlation heatmap was created to analyze relationships between numerical variables.

### 8. Profitability Analysis

Profit margin was calculated for each product category using:

**Profit Margin = (Total Profit / Total Sales) × 100**

---

## 📈 Key Findings

### Customer Demographics

- The **26–35 age group** is the largest customer segment with 1,317 customers.
- The **36–45 age group** is the second-largest segment with 1,119 customers.
- Overall, the customer base is concentrated mainly in the 26–45 age range.

### Best-Selling Products

The highest-selling products by quantity included:

1. Rice (5kg) – 1,568 units
2. Jeans – 1,563 units
3. Tennis Racket – 1,524 units
4. Jacket – 1,522 units
5. Fiction Novel – 1,519 units

### Revenue by Category

Electronics generated the highest total sales at approximately **157.17 million**, followed by Furniture and Sports.

### Correlation Analysis

Important correlations observed in the dataset include:

- Sales Amount ↔ Profit: **0.95**
- Quantity ↔ Profit: **0.66**
- Quantity ↔ Sales Amount: **0.54**
- Unit Price ↔ Sales Amount: **0.30**

### Profitability

- Beauty recorded the highest profit margin at approximately **45.19%**.
- Books recorded approximately **37.24%**.
- Clothing recorded approximately **36.09%**.
- Electronics generated the highest revenue but had a comparatively lower profit margin of approximately **12.28%**.
- Groceries had the lowest profit margin at approximately **7.85%**.

---

## 💡 Business Recommendations

1. **Optimize inventory for high-volume products**  
   Maintain adequate stock levels for products with high sales quantities to reduce the risk of stockouts.

2. **Review Electronics profitability**  
   Electronics generates the highest revenue but has a comparatively lower profit margin. Pricing, discounts, sourcing costs, and product-level margins should be reviewed.

3. **Target core customer age groups**  
   Customers aged 26–45 represent the largest customer segment, making this group suitable for targeted marketing campaigns.

4. **Consider both revenue and profitability**  
   Business decisions should consider total revenue, total profit, and profit margin together rather than relying only on revenue.

---

## 📁 Project Structure

```text
DataAnalytics-L1-Task1-RetailSalesEDA/
│
├── dataset/
│   └── retail_sales_dataset.csv
│
├── outputs/
│   ├── monthly_sales_trend.png
│   ├── quarterly_sales_trend.png
│   ├── age_group_distribution.png
│   ├── gender_distribution.png
│   ├── top_10_products.png
│   ├── revenue_by_category.png
│   ├── correlation_heatmap.png
│   └── profit_margin_by_category.png
│
├── Retail_Sales_EDA.ipynb
├── README.md
└── .gitignore