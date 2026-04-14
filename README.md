#🛒 Online Retail Data Analysis (Pandas Project)



📌 Project Overview

This project analyzes real-world e-commerce transaction data from an online retail dataset. The goal is to understand customer behavior, identify revenue patterns, analyze product performance, and gain insights into returns and seasonal trends using Python and Pandas.

🎯 Objectives

Clean and preprocess real-world transactional data
Analyze sales trends over time (monthly and daily)
Identify top-performing and high-revenue products
Perform customer segmentation based on spending behavior
Explore returned products and their impact on business


📂 Dataset Information

The dataset contains online retail transactions with the following key columns:

InvoiceNo: Transaction ID
StockCode: Product code
Description: Product name
Quantity: Number of units purchased (negative values indicate returns)
InvoiceDate: Date and time of purchase
UnitPrice: Price per unit
CustomerID: Unique customer identifier
Country: Customer location


🧹 Data Cleaning Steps


Converted InvoiceDate to datetime format
Removed missing values
Removed transactions with:
Negative quantities (returns for main analysis)
Zero unit price
Created a cleaned dataset for accurate sales analysis


⚙️ Feature Engineering


The following features were created:

Total_Price = Quantity × UnitPrice
Day = Day name of transaction
Month = Month of transaction
Year = Year of transaction


👤 Customer-Level Analysis

Computed key customer metrics:

Total Spend per Customer
Total Number of Orders
Average Order Value
Last Purchase Date
Customer Segmentation

Customers were grouped into:

High Value Customers
Medium Value Customers
Low Value Customers

(based on total spending)

📊 Exploratory Data Analysis


🕒 Time-Based Analysis

Monthly revenue trends identified peak months (holiday season effect)
Daily sales distribution analyzed to find high-performing days

🛍️ Product Analysis

Most sold products identified by quantity
Most profitable products identified by total revenue

🔄 Return Analysis

Identified products with highest return frequency
Analyzed negative quantity transactions separately
Found potential issues such as:
Product quality concerns
Customer dissatisfaction
Order mismatch

📈 Key Insights

Revenue peaks during holiday months (Nov–Dec)
A small group of products contributes to most of the revenue
Certain high-selling products also have high return rates
Customer segmentation helps identify high-value customers for targeted marketing

🧠 Tools & Libraries

Python
Pandas
NumPy

🚀 Key Learnings

Real-world data cleaning strategies
Handling missing values and incorrect transactions
Customer segmentation logic
Business-focused data analysis thinking
Time-based and product-based trend analysis

📌 Future Improvements

Add visualizations using Matplotlib / Seaborn
Perform RFM (Recency, Frequency, Monetary) analysis
Build a dashboard using Power BI or Tableau
Apply machine learning for customer segmentation
