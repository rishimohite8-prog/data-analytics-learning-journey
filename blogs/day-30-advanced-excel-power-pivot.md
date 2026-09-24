# Day 30 — Advanced Excel Power Pivot

## Overview

Today I worked with **Power Pivot in Microsoft Excel** to move beyond basic spreadsheet analysis and work with a structured data model.

The focus was on connecting multiple tables, creating relationships, writing DAX measures, and using the resulting model for interactive analysis.

## Work Completed

### 1. Connected Multiple Tables

I imported data from multiple tables into Power Pivot and prepared the data for analysis.

### 2. Built a Data Model

I created relationships between fact and dimension tables.

The model included areas such as:

* Sales
* Products
* Customers
* Dates
* Regions

This helped organize the dataset into a structure that could be used for more advanced analysis.

### 3. Created DAX Measures

I created measures for important business metrics such as:

* Total Sales
* Total Profit
* Profit Margin
* Sales Growth

Example:

```DAX
Total Sales = SUM(FactSales[Sales])
```

```DAX
Total Profit = SUM(FactSales[Profit])
```

```DAX
Profit % = DIVIDE([Total Profit], [Total Sales])
```

### 4. Pivot Table Analysis

After building the model, I used Pivot Tables and Pivot Charts to analyze the data across different dimensions.

### 5. Interactive Analysis

I added slicers and filters to make the analysis interactive and allow different views of the data.

## What I Learned

The main learning from today's work was understanding how **Power Pivot combines Excel's familiar interface with structured data modeling and DAX-based analysis**.

It was a useful step toward working with larger and more complex datasets.

## Tools Used

* Microsoft Excel
* Power Pivot
* DAX
* Pivot Tables
* Pivot Charts
* Slicers

## Conclusion

Day 30 was focused on taking Excel from basic spreadsheet analysis toward a more structured business-intelligence workflow.

**Next step: continue practicing advanced Excel features and apply them to larger datasets.**
