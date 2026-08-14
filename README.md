# Blinkit Sales Data Analysis Using PostgreSQL

## Project Overview

This project analyzes Blinkit grocery sales data using PostgreSQL to understand sales performance, product categories, outlet characteristics, customer ratings, and inventory-related metrics.

The project includes data standardization, KPI calculation, and business-oriented SQL analysis.

## Database

The project uses PostgreSQL with the database:

`blinkitdb`

The main table used for the analysis is:

`blinkit`

## Dataset

The dataset contains information about:

- Item fat content
- Item identifier
- Item type
- Outlet establishment year
- Outlet identifier
- Outlet location type
- Outlet size
- Outlet type
- Item visibility
- Item weight
- Total sales
- Rating

## Data Preparation

The project standardizes inconsistent values in the `item_fat_content` column:

- `LF` and `low fat` → `Low Fat`
- `reg` → `Regular`

Distinct fat-content values were checked after standardization.

## Key Performance Indicators (KPIs)

The following KPIs were calculated:

- Total Sales in millions
- Average Sales
- Number of Items
- Average Rating

## Sales Analysis

### Sales by Fat Content

Calculated total sales for each item fat-content category.

### Sales by Item Type

Calculated and ranked total sales across different item types.

### Fat Content by Outlet Location

Analyzed total sales by outlet location type and item fat content.

### Sales by Outlet Establishment Year

Analyzed total sales based on the outlet establishment year.

### Sales Percentage by Outlet Size

Calculated total sales and the percentage contribution of each outlet size to overall sales using a window function.

### Sales by Outlet Location

Compared total sales across different outlet location types.

### Outlet Performance Analysis

Calculated the following metrics for each outlet type:

- Total Sales
- Average Sales
- Number of Items
- Average Rating
- Average Item Visibility

## SQL Concepts Used

- `CREATE TABLE`
- `SELECT`
- `UPDATE`
- `CASE WHEN`
- `GROUP BY`
- `ORDER BY`
- `COUNT()`
- `SUM()`
- `AVG()`
- `ROUND()`
- `DISTINCT`
- Aggregate Functions
- Window Functions
- `SUM() OVER()`
- Data Standardization
- KPI Analysis
- Percentage Calculation

## Key Skills Demonstrated

- PostgreSQL Data Analysis
- Data Standardization
- Sales Analysis
- KPI Analysis
- Product Analysis
- Outlet Performance Analysis
- Customer Rating Analysis
- SQL Aggregation
- Window Functions
- Business-Oriented Data Analysis

## Project Files

- `blinkit EtoE proj 3 pgsql.sql` — PostgreSQL queries used for data preparation, KPI calculation, and Blinkit sales analysis
- `BlinkIT Grocery Data.xlsx` — Dataset used for the analysis

## Project Structure

```text
blinkit-sales-sql-analysis/
│
├── README.md
├── blinkit EtoE proj 3 pgsql.sql
└── BlinkIT Grocery Data.xlsx
