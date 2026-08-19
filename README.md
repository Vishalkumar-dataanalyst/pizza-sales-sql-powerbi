# 🍕 Pizza Sales Analysis | SQL & Power BI

## 📌 Project Overview

This project focuses on analyzing **48,605 pizza sales transactions** using **SQL and Microsoft Power BI** to identify sales trends, product performance, customer ordering patterns, and key business KPIs.

SQL was used to perform data analysis and answer business-driven questions, while Power BI was used to build an interactive dashboard for visualizing sales performance and generating actionable insights.

The project demonstrates an end-to-end **Data Analytics workflow**, from raw transactional data to data cleaning, SQL analysis, KPI development, visualization, and business insights.

---

## 🎯 Project Objectives

The key objectives of this project were to:

* Analyze overall sales and order performance
* Calculate important business KPIs
* Identify top and low-performing pizza products
* Analyze sales by pizza category
* Analyze sales by pizza size
* Identify monthly sales trends
* Analyze order patterns across weekdays
* Identify the Top 10 pizzas based on sales
* Build an interactive Power BI dashboard
* Convert raw transactional data into meaningful business insights

---

## 📊 Dataset

The dataset contains **48,605 sales records** related to pizza orders.

### Key Columns

| Column              | Description                         |
| ------------------- | ----------------------------------- |
| `pizza_id`          | Unique pizza transaction identifier |
| `order_id`          | Unique order identifier             |
| `pizza_name_id`     | Pizza product identifier            |
| `quantity`          | Number of pizzas ordered            |
| `order_date`        | Date of the order                   |
| `order_time`        | Time of the order                   |
| `unit_price`        | Price per pizza                     |
| `total_price`       | Total transaction value             |
| `pizza_size`        | Size of the pizza                   |
| `pizza_category`    | Pizza category                      |
| `pizza_ingredients` | Pizza ingredients                   |
| `pizza_name`        | Pizza product name                  |
| `Month Name`        | Month extracted from order date     |

---

## 🛠️ Tools & Technologies

* **SQL** – Data querying and business analysis
* **Microsoft Power BI** – Interactive dashboard development
* **Power Query** – Data cleaning and transformation
* **DAX** – KPI and analytical measure creation
* **Excel/CSV** – Dataset handling
* **GitHub** – Version control and project documentation

---

# 📈 Power BI Dashboard

The interactive dashboard provides a consolidated view of pizza sales performance.

### Key KPIs

* **Total Sales**
* **Total Orders**
* **Average Order Value**
* **Total Pizza Sold**
* **Average Pizza per Order**

### Dashboard Analysis

The dashboard includes:

* 📈 Monthly Sales Trend
* 🍕 Sales Distribution by Pizza Category
* 📏 Sales Distribution by Pizza Size
* 📅 Total Orders by Weekday
* 🏆 Top 10 Pizzas by Sales
* 📊 Top Pizza by Sales
* 📉 Worst Performing Pizza
* 🎛️ Interactive filters for month, category, and pizza size

---

# 💻 SQL Analysis

SQL was used to answer important business questions from the transactional dataset.

### Total Sales

```sql
SELECT SUM(total_price) AS total_sales
FROM pizza_sales;
```

### Total Orders

```sql
SELECT COUNT(DISTINCT order_id) AS total_orders
FROM pizza_sales;
```

### Total Pizzas Sold

```sql
SELECT SUM(quantity) AS total_pizzas_sold
FROM pizza_sales;
```

### Average Order Value

```sql
SELECT 
    SUM(total_price) / COUNT(DISTINCT order_id) AS avg_order_value
FROM pizza_sales;
```

### Sales by Category

```sql
SELECT 
    pizza_category,
    SUM(total_price) AS total_sales
FROM pizza_sales
GROUP BY pizza_category
ORDER BY total_sales DESC;
```

### Sales by Pizza Size

```sql
SELECT 
    pizza_size,
    SUM(total_price) AS total_sales
FROM pizza_sales
GROUP BY pizza_size
ORDER BY total_sales DESC;
```

### Top 10 Pizzas by Sales

```sql
SELECT 
    pizza_name,
    SUM(total_price) AS total_sales
FROM pizza_sales
GROUP BY pizza_name
ORDER BY total_sales DESC
FETCH FIRST 10 ROWS ONLY;
```

> SQL syntax can be adapted according to the database system being used.

---

# 🔎 Business Questions Answered

The analysis focuses on questions such as:

1. What is the total revenue generated?
2. How many unique orders were placed?
3. How many pizzas were sold?
4. What is the average order value?
5. Which pizzas generate the highest revenue?
6. Which pizzas have comparatively low sales?
7. Which pizza category performs best?
8. Which pizza size contributes most to sales?
9. How do sales change month by month?
10. Which weekdays have the highest order volume?
11. Which are the Top 10 pizzas by sales?
12. How do customer ordering patterns vary across products and sizes?

---

# 💡 Key Analytical Insights

The analysis helps identify:

* High-performing and low-performing products
* Customer preferences for pizza categories and sizes
* Monthly sales patterns
* Weekly order patterns
* Revenue contribution by product
* Products that may require promotional attention
* Product and inventory planning opportunities

These insights can support data-driven decisions related to **sales strategy, product promotion, inventory planning, and business performance monitoring**.

---

# 🔄 Project Workflow

```text
Raw Transaction Data
        ↓
Data Cleaning & Transformation
        ↓
Exploratory Data Analysis
        ↓
SQL Business Queries
        ↓
DAX KPI Measures
        ↓
Power BI Visualizations
        ↓
Interactive Dashboard
        ↓
Business Insights
```

---

# 📁 Repository Structure

```text
Pizza-Sales-SQL-PowerBI-Analysis/
│
├── Dataset/
│   └── pizza_sales.csv
│
├── SQL/
│   └── pizza_sales_analysis.sql
│
├── PowerBI/
│   └── Pizza_Sales_Dashboard.pbix
│
├── Screenshots/
│   └── pizza_sales_dashboard.png
│
└── README.md
```

---

# 🧠 Skills Demonstrated

### SQL

* SELECT
* WHERE
* GROUP BY
* ORDER BY
* Aggregate Functions
* SUM()
* COUNT()
* AVG()
* DISTINCT
* Filtering
* Business-oriented SQL queries

### Power BI

* Power Query
* Data Transformation
* DAX Measures
* KPI Cards
* Slicers
* Line Charts
* Donut Charts
* Treemap
* Interactive Dashboard Design

### Data Analytics

* Data Cleaning
* Exploratory Data Analysis
* KPI Analysis
* Trend Analysis
* Product Performance Analysis
* Category Analysis
* Business Insight Generation

---

# 📚 Learning Outcomes

This project strengthened my practical understanding of:

* SQL-based data analysis
* Data cleaning and transformation
* KPI development
* Power BI dashboard development
* DAX calculations
* Exploratory data analysis
* Business problem solving
* Data-driven decision making

The project demonstrates the complete process of transforming raw transactional data into an interactive analytical solution.

---
## 📸 Dashboard Preview



# 👨‍💻 Author

**Vishal Kumar**

**B.Tech CSE | Aspiring Data Analyst**

### Technical Skills

`SQL` `Power BI` `Excel` `Power Query` `DAX` `Python` `Data Analytics`

---

⭐ If you find this project useful, feel free to star the repository.
