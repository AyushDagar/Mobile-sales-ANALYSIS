# 📊 Power BI Sales Dashboard Project

This is an end-to-end Power BI project that visualizes and analyzes sales data using interactive dashboards. The project includes **data transformation**, **DAX measures**, **relationship modeling**, and **business insights**.

![Dashboard Screenshot](images/sales-dashboard.png) <!-- Optional: Add a screenshot to /images folder -->

---

## 📁 Project Files

- `SalesDashboardProject.pbix` – Main Power BI dashboard file
- `/data/` – Raw source data files (CSV/Excel)
- `/images/` – Dashboard screenshots (optional)
- `README.md` – Project documentation

---

## 🔧 Data Cleaning & Transformation (Power Query)

Performed inside Power BI using Power Query Editor:

- Removed irrelevant columns
- Changed data types (e.g., Date, Text, Whole Number)
- Removed duplicates and filtered out null values
- Merged related tables (Customer, Product, Region)
- Extracted Year, Month, Quarter from Date column
- Replaced values for consistency (e.g., region names)
- Created conditional columns for status/category

---

## 🔢 DAX Measures Used

```DAX
Total Sales = SUM(Sales[SalesAmount])
Total Profit = SUM(Sales[Profit])
Total Quantity = SUM(Sales[Quantity])
Sales LY = CALCULATE([Total Sales], SAMEPERIODLASTYEAR('Date'[Date]))
Sales Growth = [Total Sales] - [Sales LY]
Sales Growth % = DIVIDE([Sales Growth], [Sales LY])
Profit Margin = [Total Profit] / [Total Sales]
---

## 📊 Visuals Included

- KPI Cards (Total Sales, Total Profit, Quantity Sold)
- Clustered Bar Chart (Sales by Product Category)
- Pie Chart (Customer Segment Distribution)
- Line Chart (Monthly Sales Trend)
- Map Visual (Sales by Country/Region)
- Table with Conditional Formatting
- Slicers for dynamic filtering (Date, Category, Region)

---

## 📈 Dashboard Insights

- Identified top-performing and underperforming product categories
- Analyzed profit margins across products and regions
- Tracked monthly and quarterly sales growth over time
- Visualized regional sales performance on a map
- Compared sales by customer segments to understand buying behavior
- Monitored year-over-year growth using DAX time intelligence

---

## 🚀 Tools Used

- Power BI Desktop
- Power Query Editor
- DAX (Data Analysis Expressions)

---

## 📬 Contact

- 📧 Email: [your_email@example.com]
- 🔗 LinkedIn: [https://www.linkedin.com/in/your-profile/]
