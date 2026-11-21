# Customer Data Cleaning & Preparation

## Project Overview
This project focuses on cleaning and preparing the Customer Personality Analysis dataset from Kaggle using Python and Pandas.

The objective was to identify and handle missing values, duplicate records, incorrect data types, and inconsistent values to make the dataset ready for further analysis.

## Dataset Information
- Dataset: Customer Personality Analysis
- Original records: 2,240 rows
- Original columns: 29
- Tool used: Python
- Library used: Pandas and NumPy

## Data Cleaning Performed

### 1. Missing Values
- Identified 24 missing values in the Income column.
- Replaced missing Income values with the median.
- Verified that no missing values remained.

### 2. Duplicate Records
- Checked for duplicate rows.
- No duplicate rows were found.
- Verified that all customer IDs were unique.

### 3. Data Type Correction
- Converted the Dt_Customer column from object/string to datetime format.

### 4. Inconsistent Values
- Checked Education and Marital_Status for unnecessary leading or trailing spaces.
- No extra spaces were found.
- Preserved unusual or rare categories rather than changing values without confirmation.

### 5. Anomaly Detection
- Identified three potentially unusual birth years: 1893, 1899, and 1900.
- Added a Birth_Year_Flag column to mark these records for review.
- Retained the original birth-year values.

## Final Dataset Results
- Total rows: 2,240
- Total columns: 30
- Missing values: 0
- Duplicate rows: 0
- Duplicate customer IDs: 0
- Birth-year records flagged for review: 3

## Files Included
- `cleaned_customer_data.csv` – Final cleaned dataset.
- `customer_data_cleaning.ipynb` – Python notebook containing the cleaning process.

## Conclusion
The dataset was successfully cleaned and prepared using Python. Missing values were handled, data types were corrected, duplicate records were checked, and unusual birth years were flagged for further review. The final dataset is ready for further analysis.
