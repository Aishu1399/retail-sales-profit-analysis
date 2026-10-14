# Retail Sales & Profit Analysis Dashboard

An end-to-end data analytics portfolio project using **Microsoft Excel, SQL Server, and Power BI** to analyze retail sales, profitability, product performance, customer segments, and regional trends.

> **Note:** This project uses sample data for portfolio and learning purposes. The results do not represent an actual company's sales or financial performance.

## Table of Contents
- [Project Overview](#project-overview)
- [Business Objectives](#business-objectives)
- [Tools and Technologies](#tools-and-technologies)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Key Performance Indicators](#key-performance-indicators)
- [Dashboard Pages](#dashboard-pages)
- [Dashboard Screenshots](#dashboard-screenshots)
- [Key Business Insights](#key-business-insights)
- [SQL Analysis](#sql-analysis)
- [Excel Analysis](#excel-analysis)
- [Skills Demonstrated](#skills-demonstrated)

## Project Overview
The goal is to turn retail transaction data into useful business insights. The workflow covers data preparation in Excel, querying and analysis in SQL Server, and interactive reporting in Power BI.

The report contains three pages:
1. Executive Sales Overview
2. Product & Profitability Analysis
3. Regional Sales & Profit Analysis

## Business Objectives
- Monitor sales, profit, order count, profit margin, and average order value.
- Compare sales and profit across categories and sub-categories.
- Identify top 10 products by sales and bottom 10 products by profit.
- Examine monthly sales trends across 2024 and 2025.
- Compare regional and state-level performance.
- Understand sales contribution by customer segment.
- Explore results using year, region, category, and segment filters.

## Tools and Technologies
| Tool | How it was used |
|---|---|
| Microsoft Excel | Data checks, XLOOKUP, calculated columns, PivotTables, and exploratory analysis |
| Microsoft SQL Server | Aggregations, GROUP BY, CTEs, window functions, and business questions |
| Power Query | Data preparation and shaping |
| Power BI | Interactive reports, visualizations, slicers, and report layout |
| DAX | KPI measures and calendar/date calculations |

## Dataset
The sample dataset covers **2024–2025** and contains:
- **5,000** sales transactions
- **500** customers
- **20** products

The analysis uses sales, profit, quantity, order date, product, category, region, state, and customer segment fields.

## Project Workflow

### 1. Excel: Data Preparation and Exploratory Analysis
- Checked data quality, blanks, duplicates, and data types.
- Used `XLOOKUP` to bring product and customer attributes into the sales analysis.
- Created Year, Month Number, Month, Year-Month, and Profit Margin columns.
- Built PivotTables for KPIs, category/sub-category performance, region, customer segment, top products, low-profit products, and monthly trends.

### 2. SQL Server: Business Analysis
Created queries to answer questions such as:
- What are total sales, profit, quantity sold, and order count?
- Which categories and regions generate the highest sales and profit?
- Which products are the top 10 by sales?
- Which products have the lowest profit?
- How do sales and profit change month by month?
- Which products have high sales but relatively low profit margin?
- Which category performs best within each region?
- Which customers contribute the most sales?
- How did sales and profit change year over year?

SQL concepts practiced include `SUM`, `COUNT`, `GROUP BY`, `ORDER BY`, `TOP`, CTEs, `RANK()` / window functions, `LAG()`, and percentage calculations.

### 3. Power BI: Data Modeling and Dashboarding
- Created a calendar table based on the minimum and maximum order dates.
- Established an active many-to-one relationship between sales `Order_Date` and calendar `Date`.
- Created DAX measures for sales, profit, quantity, orders, profit margin, and average order value.
- Built three report pages and synchronized the Year slicer across pages.
- Used KPI cards, charts, a matrix, and slicers for interactive exploration.

## Key Performance Indicators
The following values represent the complete sample dataset with no filters applied.

| KPI | Result |
|---|---:|
| Total Sales | ₹14,223,768 |
| Total Profit | ₹3,031,938.47 |
| Total Orders | 5,000 |
| Total Quantity | 9,618 |
| Profit Margin | 21.32% |
| Average Order Value | ₹2,844.80 |

## Dashboard Pages

### Page 1 — Executive Sales Overview
- KPI cards: Total Sales, Total Profit, Total Orders, Profit Margin, Average Order Value
- Monthly Sales Trend
- Sales by Category
- Profit by Region
- Sales by Customer Segment
- Slicers for Year, Region, Segment, and Category

### Page 2 — Product & Profitability Analysis
- Top 10 Products by Sales
- Bottom 10 Products by Profit
- Sales vs Profit by Product
- Sales by Sub-Category

### Page 3 — Regional Sales & Profit Analysis
- Sales by Region
- Profit by Region
- Sales by State
- Category Performance by Region, comparing sales and profit

## Dashboard Screenshots

### 1. Executive Sales Overview
![Executive Sales Overview](Executive%20Sales%20Overview.png)

### 2. Product & Profitability Analysis
![Product & Profitability Analysis](Product%20%26%20Profitability%20Analysis.png)

### 3. Regional Sales & Profit Analysis
![Regional Sales & Profit Analysis](Regional%20Sales%20%26%20Profit%20Analysis.png)

## Key Business Insights
Based on the full sample dataset:
- **Furniture** is the highest-sales category, generating approximately **₹59.0 lakh**.
- The **West** region leads in total sales and total profit.
- **Office Chair** is the highest-selling product by sales.
- The **Consumer** segment contributes the most sales, at approximately **₹79.94 lakh**.
- The overall profit margin is approximately **21.32%**.
- 2025 sales increased by approximately **2.45%** and profit increased by approximately **4.39%** compared with 2024.

These findings describe this sample dataset only; they should not be interpreted as actual business results.

## SQL Analysis
The SQL script contains queries for KPI summaries, category and region comparisons, product rankings, monthly trends, profit margin analysis, category-by-region ranking, customer analysis, and year-over-year growth.

**SQL script:** `retail_sales_analysis_queries.sql`

## Excel Analysis
The Excel stage includes data validation, lookup-based enrichment, calculated date and profit-margin columns, and PivotTable analysis.

**workbook filename:** `Retail_Sales_Excel_Analysis.xlsx`

## Skills Demonstrated
- Data cleaning and validation
- Excel formulas, XLOOKUP, and PivotTables
- SQL querying and aggregation
- CTEs and window functions
- KPI definition and calculation
- Power Query data preparation
- Power BI data modeling and relationships
- DAX measures and calendar tables
- Dashboard design and data visualization
- Business insight communication

---
**Author:** Aishu1399  
**Repository:** [retail-sales-profit-analysis](https://github.com/Aishu1399/retail-sales-profit-analysis)
