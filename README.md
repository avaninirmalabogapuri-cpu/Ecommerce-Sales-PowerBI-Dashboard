# Ecommerce-Sales-PowerBI-Dashboard
# E-commerce Sales Analysis and Interactive Dashboard

## 📌 Project Overview

This project focuses on analyzing e-commerce sales data and creating an interactive dashboard using Microsoft Power BI.

The dashboard provides insights into sales, profit, orders, products, customers, regions, payment methods, and customer segments. Interactive slicers, maps, charts, and bookmarks are used to make the analysis easy to explore.

## 🛠️ Tools and Technologies

- Microsoft Power BI
- DAX
- CSV Dataset
- Data Visualization
- Data Analysis

## 📊 Dataset

The project uses an e-commerce sales dataset containing information about:

- Orders
- Customers
- Products
- Sales
- Profit
- Quantity
- Discount
- Region
- State
- Customer Segment
- Payment Method
- Age Group
- Order Date

## 📈 Dashboard Pages

### 1. Executive Sales Dashboard

This page provides an overall summary of the business using:

- Total Sales
- Total Profit
- Total Orders
- Average Order Value
- Monthly Sales Trend
- Sales by Product Category
- Sales by Customer Segment
- Sales by State
- Interactive slicers

### 2. Product Analysis

This page focuses on product and regional performance.

It includes:

- Top 10 Products by Sales
- Profit by Product Category
- Discount vs Profit Analysis
- Sales by Region
- Interactive filters

### 3. Customer Analysis

This page focuses on customer-related insights.

It includes:

- Customers by Age Group
- Sales by Payment Method
- Customer Distribution by State
- Sales and Orders by Customer Segment
- Interactive filters

## 🧮 DAX Measures

The following DAX measures were created:

```DAX
Total Sales = SUM(Ecommerce_Sales_Sample_Data[Sales])

Total Profit = SUM(Ecommerce_Sales_Sample_Data[Profit])

Total Orders = DISTINCTCOUNT(Ecommerce_Sales_Sample_Data[OrderID])

Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)

Average Discount = AVERAGE(Ecommerce_Sales_Sample_Data[Discount])

Average Profit = AVERAGE(Ecommerce_Sales_Sample_Data[Profit])
