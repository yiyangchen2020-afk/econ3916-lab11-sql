# SQL for Economists — Joins, Windows and the Cardinality Trap

## Objective

In this lab, I learned how to use SQL with DuckDB to analyze data and compare SQL operations with pandas.

## Methodology

- Translated pandas operations into SQL and compared their results.
- Used LEFT JOIN to combine customer and order data.
- Applied Welch's t-test before and after joining the tables.
- Used window functions to calculate regional averages and customer rankings.
- Examined how SQL handles missing values.
- Queried a public NYC taxi dataset using DuckDB.
- Used AI to translate pandas operations into SQL and checked the results.

## Key Findings

The LEFT JOIN increased the dataset from 600 to 3,612 rows by repeating customer records. The Welch t-test changed from t = 0.07 (p = 0.9413) to t = 0.71 (p = 0.4749). This shows how duplicated observations can affect statistical results.

Window functions calculated regional averages without reducing the number of rows.

SQL returned 3 rows when filtering income values not equal to 50,000, while pandas returned 5. The difference was caused by how SQL handles NULL values.

The AI-generated SQL queries matched the pandas row counts after I revised the prompt to include missing incomes.
