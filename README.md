# World Layoffs Data Cleaning Project (SQL)

## Project Overview
This project focuses on cleaning and preparing the World Layoffs dataset using SQL in MySQL Workbench.

The raw dataset contained duplicate records, inconsistent formatting, missing values, and unnecessary fields.  
The goal of this project was to transform the data into a clean, reliable, and analysis-ready table that could be used for further exploratory analysis or reporting.

---

## Dataset
- **Name:** World Layoffs Dataset  
- **Description:** Global company layoff records including company name, industry, location, total employees laid off, percentage laid off, and layoff dates.

---

## Tools Used
- **SQL (MySQL)**
- **MySQL Workbench**

---

## Data Cleaning Process
The following steps were performed during the data cleaning process:

1. **Created a staging table**  
   - A staging table was created to preserve the original raw dataset and safely perform transformations.

2. **Removed duplicate records**  
   - Used `ROW_NUMBER()` with `PARTITION BY` inside a CTE to identify and remove duplicate rows.

3. **Standardized data values**  
   - Cleaned company names and industry fields to ensure consistent formatting.
   - Standardized date formats for proper time-based analysis.

4. **Handled NULL and blank values**  
   - Identified missing and blank values.
   - Updated or removed records where necessary to maintain data integrity.

5. **Removed unnecessary columns and rows**  
   - Eliminated columns and records that were not useful for analysis.

---

## Files in This Repository
- **`layoffs_data_cleaning.sql`**  
  Contains all SQL queries used for data cleaning, including staging table creation, duplicate removal, standardization, and null handling.

---

## Key Skills Demonstrated
- SQL data cleaning and transformation
- Common Table Expressions (CTEs)
- Window functions
- Data quality checks
- Analytical problem-solving
- Writing clean, readable SQL

---

## Next Steps
The cleaned dataset can be used for:
- Exploratory Data Analysis (EDA)
- Trend analysis of global layoffs
- Visualization and dashboard creation using tools like Tableau or Power BI
