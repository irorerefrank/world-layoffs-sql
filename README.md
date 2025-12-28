# Data Cleaning – World Layoffs Dataset (SQL / MySQL)

This project focuses on cleaning and preparing the World Layoffs dataset using SQL in MySQL Workbench.

Before doing any analysis, the dataset needed to be cleaned. The raw data contained duplicate records, inconsistent text values, missing data, and columns that were not useful for analysis. The goal of this project was to create a clean, reliable table that could be safely used for exploratory analysis.

All work was done on a staging table so the original data remained unchanged.

---

## Dataset
- **Name:** World Layoffs Dataset  
- **Description:** Global company layoff records including company name, industry, country, total layoffs, percentage laid off, funding stage, funds raised, and dates.

---

## What I Did
The main data cleaning steps included:

- Created a **staging table** to preserve the raw dataset
- Identified and removed **duplicate records** using `ROW_NUMBER()` and a CTE
- Standardized text fields such as company names and industries
- Handled **NULL and blank values**
- Removed rows and columns that were not useful for analysis
- Performed validation checks after each major step

---

## Files
- `layoffs_data_cleaning.sql` – contains all SQL queries used to clean and prepare the dataset

---

## How to Run
1. Load the raw layoffs dataset into MySQL.
2. Open MySQL Workbench.
3. Run the queries in `layoffs_data_cleaning.sql` in order.
4. The final cleaned table can then be used for analysis or visualization.

---

## Why This Step Matters
Clean data is critical for accurate analysis.  
This project ensures that the layoffs dataset is consistent, free of duplicates, and structured correctly before performing any exploratory or analytical work.

---

## Next Steps
The cleaned dataset was later used for:
- Exploratory Data Analysis (EDA) in SQL
- Identifying trends by country, industry, company, and time
