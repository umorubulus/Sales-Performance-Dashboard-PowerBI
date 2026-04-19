# 📊 Sales Performance Dashboard (Power BI)

<p align="center">
  <a href="https://github.com/umorubulus/Sales-Performance-Dashboard-PowerBI" target="_blank">
    <b>🔗 View Full Project</b>
  </a>
</p>

---

## 📌 Project Overview

This project analyzes sales performance across multiple regions, customer segments, and product categories to uncover actionable business insights.

The dashboard provides a clear view of revenue trends, customer behavior, and regional performance, enabling data-driven decision-making.

---

## 🎯 Objectives

- Analyze overall sales performance and revenue trends  
- Identify top-performing regions and customer segments  
- Understand customer purchasing behavior  
- Highlight key drivers of business growth  

---

## 📊 Dashboard Preview

<p align="center">
  <img src="images/dashboard.png" width="800"/>
</p>

---

## 🔍 Key Insights

- 📈 Revenue shows consistent growth with seasonal fluctuations  
- 🌍 Certain regions significantly outperform others in total sales  
- 👥 A small group of customers contributes a large portion of revenue  
- 🛒 High-frequency customers drive repeat business value  

---

## 🛠 Tech Stack

![Python](https://img.shields.io/badge/Python-blue?style=for-the-badge)
![SQL](https://img.shields.io/badge/SQL-lightgrey?style=for-the-badge)
![Pandas](https://img.shields.io/badge/pandas-150458?style=for-the-badge)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge)
![Power BI](https://img.shields.io/badge/Power%20BI-yellow?style=for-the-badge)
![Matplotlib](https://img.shields.io/badge/Matplotlib-orange?style=for-the-badge)
![Excel](https://img.shields.io/badge/Excel-green?style=for-the-badge)
![Git](https://img.shields.io/badge/Git-red?style=for-the-badge)
![GitHub](https://img.shields.io/badge/GitHub-black?style=for-the-badge)

---

## 🗄 Data Source

- Synthetic dataset generated for sales analysis  
- Cleaned and prepared for analytics and visualization  
- Includes customer transactions, pricing, and geographic data  

---

## ⚙️ Data Processing Workflow

1. Data collection and preparation in Excel  
2. Data cleaning and transformation  
3. Import into Power BI  
4. Data modeling and relationship setup  
5. Dashboard creation and visualization  

---

## 🗄 SQL Analysis

```sql
-- Top Customers by Revenue
SELECT 
    CustomerID,
    SUM(Quantity * UnitPrice) AS total_revenue
FROM transactions
GROUP BY CustomerID
ORDER BY total_revenue DESC
LIMIT 10;

-- Revenue by Country
SELECT 
    Country,
    SUM(Quantity * UnitPrice) AS revenue
FROM transactions
GROUP BY Country
ORDER BY revenue DESC;
