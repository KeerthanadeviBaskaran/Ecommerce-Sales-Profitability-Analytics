# E-commerce Sales & Profitability Analytics Dashboard

## 📊 Project Overview

The **E-commerce Sales & Profitability Analytics Dashboard** is an interactive Business Intelligence project developed using Microsoft Power BI. It analyzes sales, profit, order quantity, order volume, and profitability across product categories and geographical regions.

The project transforms the Sample Superstore dataset into an interactive executive dashboard that helps users monitor business performance, identify sales trends, compare product categories, and investigate areas requiring profitability improvement.

## 🎯 Objectives

- Analyze overall sales and profitability performance.
- Track monthly sales trends over time.
- Compare sales and profit across product categories.
- Evaluate sales performance across geographical regions.
- Build interactive filters for detailed data exploration.
- Identify business insights and provide data-driven recommendations.

## 🛠️ Tools and Technologies

- **Microsoft Power BI Desktop** — Dashboard development and visualization
- **Power Query** — Data inspection and preparation
- **DAX (Data Analysis Expressions)** — Calculated measures and KPI development
- **Sample Superstore Dataset** — Retail sales data for analysis

## 📁 Dataset

The project uses the Sample Superstore dataset, which contains retail transaction information.

Important fields used in the analysis include:

- Order Date
- Order ID
- Sales
- Profit
- Quantity
- Category
- Region

The dataset supports analysis of sales performance, profitability, product categories, and geographical regions.

## 📈 Dashboard Features

### 1. Key Performance Indicators (KPIs)

The dashboard includes five KPI cards:

- **Total Sales:** Overall sales revenue.
- **Total Profit:** Total profit generated.
- **Total Quantity:** Total quantity of products sold.
- **Total Orders:** Number of distinct orders.
- **Profit Margin (%):** Profit as a percentage of sales.

### 2. Monthly Sales Trend

A line chart visualizes monthly sales over time. The YearMonth field provides a chronological timeline for examining sales fluctuations and identifying periods of higher or lower sales.

### 3. Sales and Profit by Category

A category comparison chart evaluates three product categories:

- Furniture
- Office Supplies
- Technology

This visual helps compare sales volume with profit contribution and identify categories requiring further investigation.

### 4. Sales by Region

A horizontal bar chart compares sales across the available geographical regions. Sorting the regions by sales in descending order makes it easier to identify the strongest and weakest sales performers.

### 5. Interactive Slicers

The dashboard includes three interactive slicers:

- Region
- Category
- Order Date

These filters allow users to explore different segments of the data and examine how the selected filters affect the dashboard's KPIs and visualizations.

### 6. Business Insights and Recommendations

A dedicated insights section summarizes the key findings and suggests potential business actions based on the analysis.

## 🧮 DAX Measures

The following DAX measures were created for the dashboard.

### Total Sales

```dax
Total Sales =
SUM('Superstore'[Sales])
```

Calculates the total sales value.

### Total Profit

```dax
Total Profit =
SUM('Superstore'[Profit])
```

Calculates the total profit generated.

### Total Orders

```dax
Total Orders =
DISTINCTCOUNT('Superstore'[Order ID])
```

Counts the distinct order IDs.

### Total Quantity

```dax
Total Quantity =
SUM('Superstore'[Quantity])
```

Calculates the total quantity sold.

### Profit Margin %

```dax
Profit Margin % =
DIVIDE([Total Profit], [Total Sales], 0)
```

Calculates the ratio of total profit to total sales. The measure is formatted as a percentage.

### YearMonth

```dax
YearMonth =
FORMAT('Superstore'[Order Date], "YYYY-MM")
```

Creates a year-month label for the monthly sales chart. The YearMonth column is sorted chronologically using a numeric year-month sort column where needed.

## 🔍 Key Business Insights

Based on the observed dashboard values:

- **Technology:** Approximately $840K in sales and $146K in profit, making it the strongest category in both sales and total profit among the three categories.
- **Office Supplies:** Approximately $730K in sales and $126K in profit, with an estimated profit margin of 17.3%.
- **Furniture:** Approximately $750K in sales and $19K in profit, with an estimated profit margin of 2.5%.

<img width="589" height="331" alt="ECommerce_Dashboard" src="https://github.com/user-attachments/assets/2cd65695-5a4e-445f-8702-6127e886e387" />


### Recommendations

1. Investigate Furniture's low profit margin by examining product-level performance, discounting, pricing, and costs.
2. Identify the Technology products and subcategories that contribute most to sales and profit.
3. Examine the factors supporting Office Supplies' profitability and identify opportunities to maintain or improve its performance.
4. Use the interactive slicers to compare performance across regions, categories, and date ranges.

*Note: The profit margins above are approximate because they were calculated from rounded sales and profit values. These findings identify areas for further investigation and do not establish the causes of profitability differences.*

## 💡 Skills Demonstrated

- Data inspection and preparation
- Data visualization using Power BI
- DAX measure creation
- KPI development
- Time-series sales analysis
- Category and regional performance analysis
- Interactive dashboard design
- Business insight generation
- Data-driven recommendations

## 🚀 Project Outcome

This project demonstrates how Power BI can transform retail transaction data into an interactive executive dashboard. It brings key performance indicators, time-based trends, category comparisons, regional sales analysis, and business recommendations together in a single report.

The dashboard provides a practical foundation for exploring business performance and supporting data-informed decision-making.

## 👩‍💻 Author

**Keerthanadevi Baskaran**

B.Tech — Artificial Intelligence and Data Science

GitHub: [KeerthanadeviBaskaran](https://github.com/KeerthanadeviBaskaran)

LinkedIn: [Keerthanadevi Baskaran](https://www.linkedin.com/in/keerthanadevi-baskaran-0b9a68325/)
