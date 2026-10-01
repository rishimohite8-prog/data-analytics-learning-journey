# Day 35 — SQL: Working with an Orders Dataset

## Overview

Today I worked with an `orders` table in MySQL containing structured order and customer data.

The dataset includes information such as:

- Order ID
- Customer Name
- City
- Product
- Category
- Quantity
- Price per Unit
- Discount Percentage
- Order Date
- Delivery Date
- Payment Mode
- Order Status
- Rating

## SQL Work

I started by retrieving the complete dataset using:

```sql
SELECT * FROM orders;
