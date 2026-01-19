Sales Data Analysis Using SQL 📊
Project Overview

This project demonstrates Sales Data Analysis using MySQL, focusing on transforming raw sales data into actionable business insights. The analysis covers sales trends, customer behavior, product performance, and regional revenue distribution using SQL queries, window functions, and stored procedures.

The project uses a star-schema–like database design, including fact and dimension tables, to simulate real-world sales data analysis workflows.

🗂 Database Structure
Fact Table

fact_sales – Contains transactional sales data including order dates, products, customers, and sales territories.

Dimension Tables

product – Product details including name, price, and cost.

product_subcategory – Subcategories for products.

product_category – Categories for products.

customer_lookup – Customer details including birth date and full name.

territory – Sales territories and regions.

calendar – Date information for time-based analysis.

returns_data – Information about returned products.

⚙️ Tools & Technologies

MySQL 8.0

MySQL Workbench

SQL (JOINs, CTEs, Window Functions, Stored Procedures)

CSV Files (Data Sources)

🔄 Project Workflow
1️⃣ Database Creation
CREATE DATABASE sales;
USE sales;

2️⃣ Data Loading

Dimension tables – Imported via MySQL Table Data Import Wizard.

Fact table (fact_sales) – Loaded using LOAD DATA INFILE for bulk insertion:

SET GLOBAL local_infile = 1;
LOAD DATA INFILE 'C:/ProgramData/MySQL/MySQL Server 8.0/Uploads/Fact Sales Data.csv'
INTO TABLE fact_sales
FIELDS TERMINATED BY ','
OPTIONALLY ENCLOSED BY '"'
LINES TERMINATED BY '\r\n'
IGNORE 1 ROWS
(OrderDate, StockDate, OrderNumber, ProductKey, CustomerKey, TerritoryKey, OrderLineItem, OrderQuantity);

3️⃣ Data Cleaning & Transformation

Convert date columns to proper DATE format:

UPDATE calendar SET date = STR_TO_DATE(date,'%m/%d/%Y');
ALTER TABLE calendar MODIFY COLUMN date DATE;


Apply numeric data types (INT, DECIMAL) to numeric fields like ProductPrice and ProductCost.

4️⃣ Data Analysis

Used JOINs to combine fact and dimension tables.

Applied window functions (LAG, RANK, ROW_NUMBER) for trend and ranking analysis.

Created stored procedures for reusable queries.

📊 Key Analysis & Insights

Total sales quantity per product

Total sales revenue per region

Revenue per product category

Top 10 customers by spending

Total orders by region

Revenue for a given category (stored procedure)

Products sold in a date range (stored procedure)

Month-to-month sales comparison (using LAG)

Number of orders per customer (using ROW_NUMBER)

Repeat customers

Percentage of returned products

Most popular product in each category

Top-spending customer per region

Difference between product price and category average

Customers ordering from multiple territories

🧠 Advanced SQL Concepts Used

JOINs – Inner, Left, and Multi-table joins

CTE (Common Table Expressions) – For modular queries

Window Functions – LAG, RANK, ROW_NUMBER, AVG() OVER()

Stored Procedures – Dynamic and reusable queries

Aggregate Functions – SUM, COUNT, AVG

GROUP BY & HAVING – For summary and conditional aggregation

Subqueries – Nested queries for advanced insights

📁 Files Included
File	Description
sales_project.sql	Complete SQL queries, stored procedures, and data cleaning scripts
sales_project.pdf	Project report with explanations and visual insights
README.md	Project documentation
CSV Files	Raw data sources for fact and dimension tables
✅ Conclusion

This project demonstrates a comprehensive SQL workflow from database creation, data cleaning, to advanced analysis. It highlights real-world business scenarios such as sales trend monitoring, customer behavior analysis, and revenue insights—helping organizations make data-driven decisions.

👤 Author

Al Fahim Fuad
BSc in CSE, East West University
