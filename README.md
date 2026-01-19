# Sales Data Analysis Using SQL

## 📌 Project Overview
This project focuses on analyzing sales data using MySQL to extract meaningful business insights. A structured sales database was designed using fact and dimension tables, including products, customers, territories, calendar, and returns data.

The project covers the complete data analysis workflow, from data loading and cleaning to advanced SQL-based analysis.

---

## 🗂 Database Structure
The database consists of the following tables:
- Fact Table: fact_sales
- Dimension Tables:
  - product
  - customer_lookup
  - territory
  - calendar
  - returns_data
  - product_category
  - product_subcategory

---

## ⚙️ Tools & Technologies
- MySQL
- SQL
- CSV Files
- MySQL Workbench

---

## 🔄 Project Steps

### 1️⃣ Database Creation
- Created a sales database in MySQL.
- Used fact and dimension table structure for proper data modeling.

### 2️⃣ Data Loading
- Imported dimension tables using MySQL Table Data Import Wizard.
- Loaded large fact table data using `LOAD DATA INFILE` for efficient bulk loading.

### 3️⃣ Data Cleaning & Transformation
- Converted date columns into proper DATE format.
- Corrected numeric columns to appropriate data types such as INT and DECIMAL.

### 4️⃣ Data Analysis
- Wrote complex SQL queries using JOINs and CTEs.
- Used Window Functions such as LAG, RANK, and ROW_NUMBER.
- Created Stored Procedures for reusable analysis.

---

## 📊 Key Analysis & Insights
- Total sales quantity per product
- Total revenue by region
- Revenue by product category
- Top spending and repeat customers
- Monthly sales comparison
- Product return percentage
- Most popular products in each category
- Customers ordering from multiple territories

---

## 🧠 Advanced SQL Concepts Used
- JOINs
- CTE (Common Table Expressions)
- Window Functions (LAG, RANK, ROW_NUMBER)
- Stored Procedures
- Aggregate Functions
- Group By & Having
- Subqueries

---

## 📁 Files Included
- `sales_project.sql` – Complete SQL queries and procedures
- `Final_Project_SQL.pdf` – Project report and explanation
- `README.md` – Project documentation

---

## ✅ Conclusion
This project demonstrates practical SQL skills in data analysis, database management, and business reporting. It reflects real-world sales analysis scenarios and supports data-driven decision making.

