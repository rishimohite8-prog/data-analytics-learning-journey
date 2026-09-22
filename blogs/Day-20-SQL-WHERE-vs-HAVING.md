# Day 20 — Understanding WHERE vs HAVING in SQL

While working with SQL queries, I focused on understanding the difference between `WHERE` and `HAVING`.

Both are used to filter data, but they operate at different stages of a query.

`WHERE` is used to filter individual rows before grouping and aggregation. `GROUP BY` then creates groups from the filtered records. `HAVING` is used after grouping to filter those aggregated groups.

For example, when analyzing sales data, I can use `WHERE` to select transactions from a particular category or date range. After grouping the data by category, I can use `HAVING` to keep only categories whose total sales cross a particular value.

The basic flow I worked with was:

`WHERE → GROUP BY → Aggregation → HAVING`

This exercise helped me understand that SQL filtering is not just about memorizing syntax. Understanding when each clause operates makes it much easier to build and debug analytical queries.

### What I practiced

* Filtering rows with `WHERE`
* Grouping records using `GROUP BY`
* Applying aggregate functions such as `SUM()` and `COUNT()`
* Filtering grouped results using `HAVING`
* Understanding the execution flow of an analytical SQL query

**Day 20 completed — SQL filtering and aggregation practice.**
