# 📊 Sales Analytics Dashboard — Power BI Project

## 📌 Project Overview

The **Sales Analytics Dashboard** is an interactive Power BI project developed to analyze sales performance, profitability, product categories, customer segments, and shipping methods using the Sample Superstore dataset.

The dashboard transforms raw sales data into meaningful visualizations and key performance indicators (KPIs), helping users understand business performance, identify trends, and explore opportunities for improvement.

## 🎯 Project Objectives

* Analyze overall sales and profit performance.
* Monitor key business performance indicators.
* Identify top-performing products and product categories.
* Compare sales and profitability across different regions.
* Analyze sales performance by customer segment.
* Track monthly sales trends.
* Compare sales and profit across product sub-categories.
* Understand sales distribution by shipping method.
* Explore data using interactive slicers.

## 🛠️ Tools and Technologies

| Tool                       | Purpose                                      |
| -------------------------- | -------------------------------------------- |
| Microsoft Power BI Desktop | Dashboard development and data visualization |
| Power Query                | Data cleaning and transformation             |
| DAX                        | Calculations and KPI development             |
| Sample Superstore Dataset  | Source data for sales analysis               |

## 📂 Dataset Information

This project uses the Sample Superstore dataset, which contains information about orders, customers, products, shipping, sales, discounts, and profits.

### Important Dataset Columns

| Column        | Description                |
| ------------- | -------------------------- |
| Row ID        | Row identifier             |
| Order ID      | Order identifier           |
| Order Date    | Date the order was placed  |
| Ship Date     | Date the order was shipped |
| Ship Mode     | Shipping method used       |
| Customer Name | Customer's name            |
| Segment       | Customer segment           |
| Region        | Sales region               |
| Category      | Product category           |
| Sub-Category  | Product sub-category       |
| Product Name  | Product name               |
| Sales         | Sales amount               |
| Quantity      | Number of units sold       |
| Discount      | Discount applied           |
| Profit        | Profit or loss amount      |

## 🧹 Data Cleaning and Preparation

Data preparation was performed using Power Query and Power BI.

The following steps were completed:

* Reviewed column names and data types.
* Removed blank rows.
* Removed duplicate Row IDs.
* Checked and corrected column data types, including dates and numeric values.
* Created a Calendar table for date-based analysis.
* Established a relationship between the Calendar table and the Superstore table using Order Date.
* Created a Year-Month field for monthly sales analysis.
* Sorted Year-Month values chronologically to ensure the correct order on the sales trend chart.

## 📈 Key Performance Indicators (KPIs)

The dashboard includes the following KPIs:

| KPI                       | Description                               |
| ------------------------- | ----------------------------------------- |
| Total Sales               | Total sales revenue                       |
| Total Profit              | Total profit or loss                      |
| Total Orders              | Number of distinct orders                 |
| Profit Margin             | Profit expressed as a percentage of sales |
| Total Quantity Sold       | Total number of product units sold        |
| Average Order Value (AOV) | Average sales amount per distinct order   |

## 📊 Dashboard Visualizations

The dashboard contains the following visualizations:

1. **Monthly Sales Trend** — Shows how sales change over time.
2. **Sales by Product Category** — Compares sales across product categories.
3. **Sales and Profit by Region** — Compares sales and profit across geographical regions.
4. **Top 10 Products by Sales** — Displays the ten products with the highest sales.
5. **Sales by Sub-Category** — Compares sales across product sub-categories.
6. **Sales by Customer Segment** — Shows sales across Consumer, Corporate, and Home Office segments.
7. **Profit by Sub-Category** — Identifies profitable and loss-making product sub-categories.
8. **Sales by Shipping Mode** — Compares sales across different shipping methods.
9. **Profit Margin by Category** — Compares profit margins across product categories.

## 🧮 DAX Measures

The following DAX measures were created to calculate the dashboard KPIs.

### 1. Total Sales

```dax
Total Sales = SUM(Superstore[Sales])
```

Calculates the total sales amount.

### 2. Total Profit

```dax
Total Profit = SUM(Superstore[Profit])
```

Calculates the total profit or loss.

### 3. Total Orders

```dax
Total Orders = DISTINCTCOUNT(Superstore[Order ID])
```

Counts the number of distinct orders.

### 4. Profit Margin

```dax
Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)
```

Calculates profit as a proportion of sales. This measure is formatted as a percentage in Power BI.

### 5. Total Quantity

```dax
Total Quantity = SUM(Superstore[Quantity])
```

Calculates the total quantity of products sold.

### 6. Average Order Value

```dax
Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)
```

Calculates the average sales amount per distinct order.

## 🎛️ Interactive Features

The dashboard includes interactive slicers and visual interactions to explore sales performance.

* **Region Slicer:** Filters the report by sales region.
* **Category Slicer:** Filters the report by product category.
* **Date Slicer:** Filters the report by order date.
* **Interactive Charts:** Allows users to explore sales, profit, and product performance across different dimensions.

These features make it easier to compare business performance under different filter conditions.

## 💡 Business Questions Answered

The dashboard helps answer the following business questions:

1. What are the total sales and total profit?
2. How many distinct orders were placed?
3. How do sales change over time?
4. Which product category generates the highest sales?
5. Which regions contribute the most sales and profit?
6. Which ten products have the highest sales?
7. Which customer segment generates the most sales?
8. Which product sub-categories generate losses?
9. Which shipping method accounts for the highest sales?
10. Which product category has the highest profit margin?
11. How does the selected date range affect sales performance?
12. How do sales and profitability change when filtering by region or category?

## 🔍 Key Insights

The dashboard can be used to identify:

* Monthly sales trends and changes in performance.
* High-performing products and product categories.
* Differences in sales and profitability across regions.
* Customer segments that contribute to sales.
* Product sub-categories with negative profit.
* Differences between total sales and profit margin.
* Sales distribution across shipping methods.

**Note:** Specific business findings should be added after reviewing the completed dashboard. Actual values and rankings should be taken directly from the analysis rather than assumed.

## 📸 Dashboard Preview

<img width="1202" height="676" alt="image" src="https://github.com/user-attachments/assets/f5cbf31a-a4f4-4c0e-8d8f-573a421e4372" />


## 📁 Project Structure

The recommended GitHub repository structure is:

```text
https://github.com/bhumika5me/Sales-Analytics-Dashboard-Power-BI/│
├── README.md
├── Sales-Analytics-Dashboard.pbix
├── dataset/
│   └── Sample-Superstore.csv
└── screenshots/
    └── dashboard.png
```

**Note:** This is a suggested structure. Update the filenames to match the files you actually upload. Include the original dataset only if its source and license permit redistribution.

## 🚀 How to Run the Project

1. Clone or download this GitHub repository.
2. Install Microsoft Power BI Desktop.
3. Open `Sales-Analytics-Dashboard.pbix`.
4. If Power BI asks for the data source location, update the file path to the dataset.
5. Refresh the data if necessary.
6. Open the report page and explore the dashboard.
7. Use the Region, Category, and Date slicers to interact with the visualizations.

## 📚 Skills Demonstrated

This project demonstrates practical skills in:

* Data cleaning and transformation
* Power Query
* Data modeling and relationships
* DAX calculations and measures
* KPI development
* Interactive dashboard development
* Sales and profitability analysis
* Data visualization
* Business question formulation
* Analytical thinking and insight generation

## 👩‍💻 Author

**Bhumika Tamang**

Aspiring Data Analyst | SQL | Excel | Power BI

## ⭐ Conclusion

The Sales Analytics Dashboard demonstrates how Power BI can transform raw sales data into an interactive business intelligence report.

Through data preparation, data modeling, DAX measures, and interactive visualizations, this project provides a practical analysis of sales performance, profitability, products, customers, and regional trends.

It showcases foundational data analytics skills and serves as a portfolio project for demonstrating practical Power BI experience.
