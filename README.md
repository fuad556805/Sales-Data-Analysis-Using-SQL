# Sales Data Analysis Using SQL 📊

![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=database&logoColor=white)

---

## 📌 Project Overview
This project focuses on analyzing sales data using **MySQL** to generate meaningful business insights. A structured sales database was designed using **fact and dimension tables**, following a star-schema–like approach to simulate real-world sales analytics.

The project demonstrates an **end-to-end SQL workflow**, including database creation, data loading, data cleaning, advanced querying, stored procedures, and window functions.

---

## 🗂 Database Structure

### Fact Table
- **fact_sales** – Stores transactional sales data such as order date, product, customer, territory, and order quantity.

### Dimension Tables
- **product** – Product details including price and cost  
- **product_subcategory** – Product subcategory information  
- **product_category** – Product category information  
- **customer_lookup** – Customer details  
- **territory** – Sales territories and regions  
- **calendar** – Date-related information  
- **returns_data** – Returned product data  

---

## ⚙️ Tools & Technologies
- **MySQL 8.0**
- **MySQL Workbench**
- **SQL**
- **CSV Files**

---

## 🔄 Project Workflow

### 1️⃣ Database Creation
- Created a sales database in MySQL.
- Designed fact and dimension tables for structured analysis.

### 2️⃣ Data Loading
- Imported dimension tables using **MySQL Table Data Import Wizard**.
- Loaded the large fact table using **`LOAD DATA INFILE`** for efficient bulk insertion.

### 3️⃣ Data Cleaning & Transformation
- Converted date columns into proper `DATE` format.
- Corrected numeric columns to appropriate data types such as `INT` and `DECIMAL`.

### 4️⃣ Data Analysis
- Wrote complex SQL queries using **JOINs** and **CTEs**.
- Applied **window functions** such as `LAG`, `RANK`, and `ROW_NUMBER`.
- Created **stored procedures** for reusable and dynamic analysis.

---

## 📊 Key Analysis & Insights
1. Total sales quantity per product  
2. Total revenue by region  
3. Revenue by product category  
4. Top 10 customers by total spending  
5. Total orders by region  
6. Revenue for a specific category (stored procedure)  
7. Products sold within a date range (stored procedure)  
8. Month-to-month sales comparison using `LAG()`  
9. Number of orders per customer using `ROW_NUMBER()`  
10. Repeat customers analysis  
11. Percentage of returned products  
12. Most popular product in each category  
13. Top-spending customer per region  
14. Price difference between products and category average  
15. Customers ordering from multiple territories  

---

## 🧠 Advanced SQL Concepts Used
- JOINs  
- CTE (Common Table Expressions)  
- Window Functions (`LAG`, `RANK`, `ROW_NUMBER`, `AVG() OVER`)  
- Stored Procedures  
- Aggregate Functions (`SUM`, `COUNT`, `AVG`)  
- `GROUP BY` & `HAVING`  
- Subqueries  

---

## 📁 Files Included

| File Name | Description |
|----------|------------|
| `sales_project.sql` | Complete SQL queries, stored procedures, and data cleaning scripts |
| `sales_project.pdf` | Project report and explanation |
| `README.md` | Project documentation |
| CSV Files | Raw datasets for fact and dimension tables |

---

## ✅ Conclusion
This project demonstrates strong practical skills in **SQL-based data analysis**, including database design, data cleaning, advanced querying, and business-oriented reporting. It reflects real-world sales analysis scenarios and supports **data-driven decision-making**.

---

## 👤 Author
**Al Fahim Fuyad**  
BSc in Computer Science & Engineering  
East West University
