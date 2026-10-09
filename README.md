# 📊 Sales Analytics Dashboard — Power BI Project

## 📌 Project Overview

The **Sales Analytics Dashboard** is a Power BI project built to analyze sales performance, profitability, product categories, customer segments, and shipping methods using the Sample Superstore dataset.

The dashboard transforms raw sales data into interactive visualizations and key performance indicators (KPIs) to help users understand business performance and identify opportunities for improvement.

## 🎯 Project Objectives

* Analyze overall sales and profit performance.
* Track important business KPIs.
* Identify top-performing products and categories.
* Compare sales and profitability across regions.
* Understand customer segment performance.
* Analyze sales trends over time.
* Explore how shipping methods affect sales performance.

## 🛠️ Tools and Technologies

* **Microsoft Power BI Desktop** — Data visualization and dashboard development
* **Power Query** — Data cleaning and transformation
* **DAX (Data Analysis Expressions)** — Measures and calculations
* **Sample Superstore Dataset** — Sales data for analysis

## 📂 Dataset Information

The project uses the Sample Superstore dataset, which contains order, customer, product, shipping, sales, discount, and profit information.

Key columns include:

| Column        | Description                |
| ------------- | -------------------------- |
| Order ID      | Unique order identifier    |
| Order Date    | Date the order was placed  |
| Ship Date     | Date the order was shipped |
| Customer Name | Name of the customer       |
| Segment       | Customer segment           |
| Region        | Sales region               |
| Category      | Product category           |
| Sub-Category  | Product sub-category       |
| Product Name  | Name of the product        |
| Sales         | Sales amount               |
| Quantity      | Number of units sold       |
| Discount      | Discount applied           |
| Profit        | Profit or loss amount      |

## 🧹 Data Cleaning and Preparation

The following data preparation tasks were performed in Power Query and Power BI:

* Reviewed column names and data types.
* Removed blank rows.
* Checked and removed duplicate Row IDs.
* Corrected data types, including date and numeric columns.
* Created a Calendar table for date-based analysis.
* Created a relationship between the Calendar table and the Superstore table.
* Sorted Year-Month values chronologically for the monthly sales trend.

## 📈 Key Performance Indicators (KPIs)

The dashboard includes the following KPIs:

| KPI                       | Description                         |
| ------------------------- | ----------------------------------- |
| Total Sales               | Total revenue generated from orders |
| Total Profit              | Total profit earned                 |
| Total Orders              | Number of distinct orders           |
| Profit Margin             | Profit as a percentage of sales     |
| Total Quantity Sold       | Total number of product units sold  |
| Average Order Value (AOV) | Average sales value per order       |

## 📊 Dashboard Visualizations

The dashboard includes:

1. **Monthly Sales Trend** — Tracks sales performance over time.
2. **Sales by Product Category** — Compares sales across product categories.
3. **Sales and Profit by Region** — Compares regional sales and profitability.
4. **Top 10 Products by Sales** — Identifies the ten products with the highest sales.
5. **Sales by Sub-Category** — Compares sales across product sub-categories.
6. **Sales by Customer Segment** — Analyzes sales from different customer groups.
7. **Profit by Sub-Category** — Highlights profitable and loss-making sub-categories.
8. **Sales by Shipping Mode** — Compares sales across shipping methods.
9. **Profit Margin by Category** — Compares profitability relative to sales across categories.

## 🧮 DAX Measures

The following DAX measures were created for the analysis.

### 1. Total Sales

```dax
Total Sales = SUM(Superstore[Sales])
```

### 2. Total Profit

```dax
Total Profit = SUM(Superstore[Profit])
```

### 3. Total Orders

```dax
Total Orders = DISTINCTCOUNT(Superstore[Order ID])
```

### 4. Profit Margin

```dax
Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)
```

Format this measure as a percentage.

### 5. Total Quantity

```dax
Total Quantity = SUM(Superstore[Quantity])
```

### 6. Average Order Value

```dax
Average Order Value = DIVIDE([Total Sales], [Total Orders], 0)
```

## 🎛️ Interactive Features

* **Region slicer:** Filters data by sales region.
* **Category slicer:** Filters data by product category.
* **Date slicer:** Filters data by order date.
* **Interactive charts:** Allows users to explore sales and profit performance across different dimensions.

## 💡 Business Questions Answered

This dashboard helps answer questions such as:

* What are the total sales and total profit?
* How many unique orders were placed?
* How do sales change month by month?
* Which product category generates the most sales?
* Which regions contribute the most sales and profit?
* Which ten products have the highest sales?
* Which customer segment contributes the most revenue?
* Which sub-categories generate losses?
* Which shipping method accounts for the highest sales?
* Which category has the highest profit margin?

## 🔍 Key Insights

The dashboard is designed to help identify:

* Sales trends and changes over time.
* High-performing products and categories.
* Regional differences in sales and profit.
* Differences between revenue and profitability.
* Customer segments that contribute to sales.
* Product sub-categories that may need improvement.
* Shipping methods associated with higher sales.

*Actual findings should be added after reviewing the results shown in the completed dashboard.*

## 📁 Project Files

Recommended GitHub repository structure:

```text
https://github.com/bhumika5me/
│
├── README.md
├── Sales-Analytics-Dashboard.pbix
├── dataset/
│   └── Sample-Superstore.csv
└── screenshots/
    └── dashboard.png
```

*Update the file names and folders to match your actual repository. Include the dataset only if its source and license permit redistribution.*

## 🚀 How to Run the Project

1. Download or clone this repository.
2. Install Microsoft Power BI Desktop.
3. Open the `.pbix` file in Power BI Desktop.
4. If prompted, update the dataset file path or data source.
5. Refresh the data if necessary.
6. Explore the dashboard using the interactive slicers and charts.

## 📚 Skills Demonstrated

* Data cleaning and transformation
* Power Query
* Data modeling and relationships
* DAX measures
* KPI development
* Interactive dashboard design
* Sales and profitability analysis
* Data visualization
* Business-oriented analytical thinking

## 👩‍💻 Author

**Bhumika Tamang**

Aspiring Data Analyst | SQL | Excel | Power BI

## ⭐ Conclusion

This project demonstrates how Power BI can transform sales data into an interactive dashboard for business analysis. It showcases practical skills in data preparation, data modeling, DAX calculations, visualization, and deriving business insights from data.
