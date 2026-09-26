# Day 34 — Data Wrangling Using Python

Today I worked on **data wrangling using Python and Pandas**, focusing on preparing raw data for further analysis.

## Work Completed

### 1. Loading the Dataset

Loaded the raw CSV dataset using Pandas.

```python
import pandas as pd

df = pd.read_csv("sales_data.csv")
```

### 2. Handling Missing Values

Checked for missing values and handled missing values in the `Amount` column using the median.

```python
print(df.isnull().sum())

df["Amount"] = df["Amount"].fillna(
    df["Amount"].median()
)
```

### 3. Removing Duplicate Records

Removed duplicate rows from the dataset.

```python
df.drop_duplicates(inplace=True)
```

### 4. Data Type Conversion

Converted the date column into a proper datetime format and ensured numeric fields were stored correctly.

```python
df["Date"] = pd.to_datetime(df["Date"])

df["Amount"] = pd.to_numeric(
    df["Amount"],
    errors="coerce"
)
```

### 5. Cleaning Text Data

Removed unnecessary spaces from customer names.

```python
df["Customer"] = df["Customer"].str.strip()
```

### 6. Column Transformation

Created additional columns from the existing data to make the dataset more useful for analysis.

```python
df["Month"] = df["Date"].dt.strftime("%Y-%m")
```

## Final Check

After cleaning and transformation, I verified the structure and data types of the DataFrame.

```python
print(df.info())
print(df.head())
```

The final dataset was cleaner, consistent, and ready for the next stage of analysis.

## Key Learning

Data wrangling is an important step before analysis because raw datasets often contain missing values, duplicates, inconsistent data types, and formatting issues.

**Day 34 completed — Data Wrangling using Python and Pandas.**
