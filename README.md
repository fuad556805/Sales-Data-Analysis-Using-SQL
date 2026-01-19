````markdown
# Sales Data Analysis Using SQL 📊

![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=sql&logoColor=white)

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Database Structure](#database-structure)
3. [Tools & Technologies](#tools--technologies)
4. [Project Workflow](#project-workflow)
    - [Database Creation](#database-creation)
    - [Data Loading](#data-loading)
    - [Data Cleaning & Transformation](#data-cleaning--transformation)
    - [Data Analysis](#data-analysis)
5. [Key Analysis & Insights](#key-analysis--insights)
6. [Advanced SQL Concepts Used](#advanced-sql-concepts-used)
7. [Files Included](#files-included)
8. [Conclusion](#conclusion)
9. [Author](#author)

---

## Project Overview

This project demonstrates **Sales Data Analysis** using **MySQL**, focusing on transforming raw sales data into actionable business insights. The analysis covers **sales trends, customer behavior, product performance, and regional revenue distribution** using SQL queries, window functions, and stored procedures.

The project uses a **star-schema–like database design**, including fact and dimension tables, to simulate real-world sales data analysis workflows.

---

## Database Structure

### Fact Table
- **fact_sales** – Contains transactional sales data including order dates, products, customers, and sales territories.

### Dimension Tables
- **product** – Product details including name, price, and cost.
- **product_subcategory** – Subcategories for products.
- **product_category** – Categories for products.
- **customer_lookup** – Customer details including birth date and full name.
- **territory** – Sales territories and regions.
- **calendar** – Date information for time-based analysis.
- **returns_data** – Information about returned products.

---

## Tools & Technologies
- **MySQL 8.0**
- **MySQL Workbench**
- **SQL (JOINs, CTEs, Window Functions, Stored Procedures)**
- **CSV Files (Data Sources)**

---

## Project Workflow

### Database Creation
```sql
CREATE DATABASE sales;
USE sales;
````

### Data Loading

1. **Dimension tables** – Imported via MySQL Table Data Import Wizard.
2. **Fact table (`fact_sales`)** – Loaded using `LOAD DATA INFILE` for bulk insertion.

### Data Cleaning & Transformation

* Convert date columns to proper `DATE` format.
* Apply numeric data types (`INT`, `DECIMAL`) to numeric fields like `ProductPrice` and `ProductCost`.

### Data Analysis

* Used **JOINs** to combine fact and dimension tables.
* Applied **window functions** (`LAG`, `RANK`, `ROW_NUMBER`) for trend and ranking analysis.
* Created **stored procedures** for reusable queries.

---

## Key Analysis & Insights

1. Total sales quantity per product
2. Total sales revenue per region
3. Revenue per product category
4. Top 10 customers by spending
5. Total orders by region
6. Revenue for a given category (stored procedure)
7. Products sold in a date range (stored procedure)
8. Month-to-month sales comparison (using LAG)
9. Number of orders per customer (using ROW_NUMBER)
10. Repeat customers
11. Percentage of returned products
12. Most popular product in each category
13. Top-spending customer per region
14. Difference between product price and category average
15. Customers ordering from multiple territories

---

## Advanced SQL Concepts Used

* **JOINs**
* **CTE (Common Table Expressions)**
* **Window Functions** – `LAG`, `RANK`, `ROW_NUMBER`, `AVG() OVER()`
* **Stored Procedures**
* **Aggregate Functions** – `SUM`, `COUNT`, `AVG`
* **GROUP BY & HAVING**
* **Subqueries**

---

## Files Included

| File                | Description                                                        |
| ------------------- | ------------------------------------------------------------------ |
| `sales_project.sql` | Complete SQL queries, stored procedures, and data cleaning scripts |
| `sales_project.pdf` | Project report with explanations and visual insights               |
| `README.md`         | Project documentation                                              |
| CSV Files           | Raw data sources for fact and dimension tables                     |

---

## Conclusion

This project demonstrates a **comprehensive SQL workflow** from database creation, data cleaning, to advanced analysis. It highlights **real-world business scenarios** such as sales trend monitoring, customer behavior analysis, and revenue insights—helping organizations make **data-driven decisions**.

---

## Author

**Al Fahim Fuad**
BSc in CSE, East West University

```
