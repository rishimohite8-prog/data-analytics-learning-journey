# Day 41 — SQL: Different Keys in Database Training

## Overview

Today I practiced database design in SQL by working with different types of keys and understanding their role in maintaining structured and reliable relational databases.

The practical examples were based on related tables such as:

* Employees
* Departments
* Projects
* EmployeeProjects

## Types of Keys Practiced

### 1. Primary Key

A primary key uniquely identifies each record in a table.

Example:

```sql
EmployeeID INT PRIMARY KEY
```

It ensures that each employee can be uniquely identified.

### 2. Foreign Key

A foreign key establishes a relationship between tables.

For example, an employee can reference a department through a department identifier.

```sql
DepartmentID INT,
FOREIGN KEY (DepartmentID)
REFERENCES Departments(DepartmentID)
```

### 3. Unique Key

A UNIQUE constraint prevents duplicate values in a column where values are expected to be unique.

```sql
Email VARCHAR(100) UNIQUE
```

### 4. Composite Key

A composite key uses multiple columns together to uniquely identify a record.

This is particularly useful in relationship tables such as `EmployeeProjects`.

```sql
PRIMARY KEY (EmployeeID, ProjectID)
```

### 5. Candidate Key

A candidate key is a column or combination of columns that can potentially uniquely identify records.

A table can have multiple candidate keys, but only one is selected as the primary key.

### 6. Alternate Key

An alternate key is a candidate key that was not selected as the primary key but can still uniquely identify a record.

## Database Structure

The exercise used a relational structure similar to:

```text
Employees
    |
    | DepartmentID
    ↓
Departments

Employees
    |
    | EmployeeID
    ↓
EmployeeProjects
    ↑
    | ProjectID
    |
Projects
```

This structure demonstrates how keys help establish relationships between entities.

## Key Learning

Good database design starts with correctly identifying entities and relationships.

Keys help provide:

* Entity integrity
* Referential integrity
* Duplicate prevention
* Reliable table relationships
* Better query accuracy

Without appropriate keys, databases can become inconsistent and analytical results can become unreliable.

## Conclusion

This exercise strengthened my understanding of relational database design and the practical role of different keys in SQL.

Understanding keys is fundamental not only for database development but also for reliable data analytics and data engineering.
