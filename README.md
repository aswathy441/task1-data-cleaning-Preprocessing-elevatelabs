# Elevate Labs Data Analyst Intern Task 1: Data Cleaning and Preprocessing

## Objective
Clean and prepare a raw dataset containing nulls, duplicates, and inconsistent formats to make it ready for analysis.

## Tools Used
- Python (Pandas)
- Excel (optional)

## Steps Performed

1. **Identify and Handle Missing Values**
   - Checked for missing values using `df.isnull().sum()`.
   - Handled missing values by:
     - Filling with median/mean for numeric columns.
     - Filling with default values or mode for categorical columns.
     - Dropping rows when appropriate.

2. **Remove Duplicate Rows**
   - Identified duplicates using `df.duplicated()`.
   - Removed duplicates with `df.drop_duplicates()`.

3. **Standardize Text Values**
   - Converted gender, country names, and other categorical columns to consistent formats.
   - Examples: `Male` / `Female`, `USA`, `UK`.

4. **Convert Date Formats**
   - Converted date columns to a consistent `datetime` format using `pd.to_datetime()`.

5. **Rename Column Headers**
   - Made all column headers lowercase and replaced spaces with underscores for consistency.

6. **Check and Fix Data Types**
   - Converted columns to appropriate types:
     - Age → integer
     - Salary → numeric
     - Date columns → datetime

## Deliverables
- `raw_data.csv` — Original dataset  
- `cleaned_data.csv` — Cleaned and preprocessed dataset  
- `data_cleaning.ipynb` — Python code notebook  
- `screenshots/` — Optional: screenshots showing data checks or visualizations  

## Summary of Changes
- Removed duplicate rows.  
- Handled missing values in key columns.  
- Standardized text values for consistency.  
- Converted dates to a uniform format.  
- Renamed columns for clarity and uniformity.  
- Corrected data types for proper analysis.
