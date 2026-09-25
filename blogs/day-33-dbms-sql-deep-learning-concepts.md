# Day 33 — DBMS, SQL & Deep Learning Concepts

## Overview

Today I worked on three important areas: SQL joins, database normalization, and backpropagation in deep learning.

The goal was to understand both how structured data is organized and queried, and how neural networks learn from errors.

---

## 1. SQL Joins

SQL joins are used to combine rows from two or more tables using a related column or key.

### INNER JOIN

Returns only the records that have matching values in both tables.

```sql
SELECT e.name, d.department_name
FROM employees e
INNER JOIN departments d
    ON e.department_id = d.department_id;
