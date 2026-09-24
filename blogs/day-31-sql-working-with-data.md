# Day 31 — SQL Working With Data

## Overview

Today I worked with a dataset directly in **SQL**, focusing on using queries to explore, clean, aggregate and analyze data.

Instead of practicing SQL commands individually, I worked through a complete data-analysis workflow.

## Work Completed

### 1. Dataset Exploration

I first explored the available columns and records to understand the structure of the dataset.

The dataset contained fields related to:

* Orders
* Customers
* Products
* Categories
* Sales
* Profit

### 2. Data Cleaning

I worked on preparing the data for analysis by checking data quality, handling missing values and identifying duplicate or inconsistent records.

### 3. Aggregation

I used SQL aggregate functions such as:

* `SUM()`
* `COUNT()`
* `AVG()`

These helped calculate useful metrics from the raw records.

### 4. GROUP BY Analysis

I grouped records to compare performance across categories and products.

Example:

```SQL
SELECT
    category,
    SUM(sales) AS total_sales
FROM orders
GROUP BY category
ORDER BY total_sales DESC;
```

### 5. Finding Top Products

I also worked on queries to identify products generating the highest sales.

```SQL
SELECT
    product_name,
    SUM(sales) AS total_sales
FROM orders
GROUP BY product_name
ORDER BY total_sales DESC
LIMIT 5;
```

### 6. Views

I explored creating SQL views to keep commonly used analysis queries structured and easier to reuse.

## What I Learned

Today's work helped me understand how SQL can be used as an actual **data-analysis tool**, rather than simply as a collection of commands.

The workflow was:

**Explore → Clean → Query → Aggregate → Analyze**

## Tools and Concepts

* SQL
* SELECT
* WHERE
* GROUP BY
* ORDER BY
* Aggregate Functions
* Views
* Data Cleaning

## Conclusion

Day 31 was focused on becoming more comfortable with working directly on structured data through SQL queries.

The next step is to work with more complex queries involving joins, subqueries, CTEs and window functions.
