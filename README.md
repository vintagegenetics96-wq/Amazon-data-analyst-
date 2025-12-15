# Amazon-data-analyst-
# 📦 Amazon Data Analyst Project

## 📌 Project Overview

This project analyzes Amazon-style e-commerce data to uncover insights related to sales performance, customer behavior, product trends, and delivery efficiency. The analysis supports data-driven decision-making for business growth and operational improvement.

---

## 🎯 Project Objectives

* Analyze overall sales and revenue trends
* Identify top-performing products and categories
* Measure customer lifetime value and repeat behavior
* Track delivery performance and order status
* Create KPIs for business reporting

---

## 📊 Dataset Description

This project uses **simulated Amazon e-commerce data** structured across multiple tables:

### Tables Used

* **Customers** – Customer details and signup data
* **Products** – Product category, pricing, and ratings
* **Orders** – Order dates, delivery dates, status, and payment mode
* **Order_Items** – Product-level sales with quantity and discounts

---

## 🔑 Key Business Questions

* Which product categories generate the highest revenue?
* Who are the top customers by lifetime value?
* What are the monthly sales trends?
* Which products have high ratings but low sales?
* What is the average delivery time?
* Which regions contribute most to revenue?

---

## 📈 KPIs & Metrics

* Total Revenue
* Average Order Value (AOV)
* Customer Lifetime Value (CLV)
* Monthly Sales Growth
* Order Cancellation Rate
* Average Delivery Time

---

## 🛠 Tools & Technologies

* **SQL (MySQL)** – Data extraction and analysis
* **Excel** – Data cleaning and pivot analysis
* **Power BI** – Interactive dashboards
* **GitHub** – Version control and portfolio hosting

---

## 📌 Sample SQL Queries

### Total Revenue

```sql
SELECT SUM(p.price * oi.quantity - oi.discount) AS total_revenue
FROM order_items oi
JOIN products p ON oi.product_id = p.product_id;
```

### Top 5 Best-Selling Categories

```sql
SELECT p.category, SUM(oi.quantity) AS total_sold
FROM order_items oi
JOIN products p ON oi.product_id = p.product_id
GROUP BY p.category
ORDER BY total_sold DESC
LIMIT 5;
```

---

## 📊 Dashboard Insights (Power BI)

* Sales Overview Dashboard
* Customer Analysis Dashboard
* Product Performance Dashboard
* Delivery & Logistics Dashboard
* Geographic Revenue Analysis

---

## 📂 Repository Structure

```
Amazon-Data-Analytics/
│
├── Dataset/
│   └── amazon_data.csv
├── SQL/
│   └── amazon_analysis.sql
├── PowerBI/
│   └── amazon_dashboard.pbix
├── Excel/
│   └── amazon_analysis.xlsx
├── Report/
│   └── Amazon_Data_Analyst_Project_Report.pdf
├── README.md
```

---

## 📌 Conclusion

This project demonstrates practical data analytics skills using SQL, Excel, and Power BI to analyze large-scale e-commerce data. The insights help businesses improve sales strategy, customer retention, and delivery efficiency.

---

## 👤 Author

**Yash**
📧 Email: [vintagegenetics96@gmail.com](mailto:vintagegenetics96@gmail.com)
📊 Role: Data Analyst

---

⭐ *If you find this project useful, feel free to star the repository!*
