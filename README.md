Sales Data Analysis Using SQL
📌 Project Overview

This project focuses on analyzing sales data using MySQL to generate meaningful business insights. A structured sales database was designed using fact and dimension tables, including products, customers, territories, calendar, and returns data.

The project demonstrates a complete SQL data analysis workflow—from data loading and cleaning to advanced querying and reporting.

🗂 Database Structure

The database follows a star-schema–like design and includes:

Fact Table

fact_sales

Dimension Tables

product

customer_lookup

territory

calendar

returns_data

product_category

product_subcategory

⚙️ Tools & Technologies

MySQL

SQL

MySQL Workbench

CSV Files

🔄 Project Workflow
1️⃣ Database Creation

Created a sales database in MySQL.

Designed fact and dimension tables for structured and efficient analysis.

2️⃣ Data Loading

Imported dimension tables using MySQL Table Data Import Wizard.

Loaded large fact table data using LOAD DATA INFILE for fast bulk insertion.

3️⃣ Data Cleaning & Transformation

Converted date columns into proper DATE format.

Updated numeric fields to correct data types such as INT and DECIMAL.

4️⃣ Data Analysis

Wrote complex SQL queries using JOINs and CTEs.

Applied window functions such as LAG, RANK, and ROW_NUMBER.

Created stored procedures for reusable and dynamic analysis.

📊 Key Analysis & Insights

Total sales quantity per product

Total revenue by region

Revenue by product category

Top-spending and repeat customers

Month-to-month sales comparison

Product return percentage

Most popular products in each category

Customers ordering from multiple territories

🧠 Advanced SQL Concepts Used

JOINs

CTE (Common Table Expressions)

Window Functions (LAG, RANK, ROW_NUMBER)

Stored Procedures

Aggregate Functions

GROUP BY & HAVING

Subqueries

📁 Files Included

sales_project.sql – Complete SQL queries and stored procedures

sales_project.pdf – Project report and explanation

README.md – Project documentation

✅ Conclusion

This project demonstrates strong practical skills in SQL, including database design, data cleaning, advanced querying, and business-oriented analysis. It reflects real-world sales analysis scenarios and supports data-driven decision-making.


## 👤 Author
Al Fahim Fuyad
BSc in CSE, East West University
