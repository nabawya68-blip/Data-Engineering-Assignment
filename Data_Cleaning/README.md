# Data Cleaning – Data Engineering Assignment

## 1. Project Overview

This project focuses on cleaning, validating, and integrating five datasets using Python.

## 2. Datasets

- customers_master.csv
- products_master.csv
- orders.csv
- new_daily_batch.csv
- previous_days_summary.csv

## 3. Libraries Used

- Pandas
- NumPy

## 4. Data Inspection

The datasets were inspected using:
- Shape
- Data Types
- Missing Values
- Duplicate Records
- Data Preview

## 5. Data Cleaning Steps

### Customers Dataset
- Standardized Region values.
- Standardized Customer Segment values.
- Checked missing values and duplicates.

### Products Dataset
- Standardized Category values.
- Checked data types and duplicates.

### Orders and New Daily Batch
- Standardized text columns.
- Converted dates to datetime.
- Converted numeric columns.
- Validated Quantity and Discount.
- Identified invalid dates.
- Removed exact duplicate rows.

### Previous Days Summary
- Converted Date to datetime.
- Validated numeric columns.
- Checked rate values and duplicate dates.

## 6. Data Integration

- Combined Orders and New Daily Batch using Pandas concat.
- Merged customer information using Customer_ID.
- Merged product information using Product_ID.
- Used Left Join to preserve order records.
- Identified unmatched customer and product records.

## 7. Data Quality Results

Combined dataset:
- 1,347 rows
- 21 columns

Customer matching:
- 1,336 matched records
- 11 unmatched records

Product matching:
- 1,341 matched records
- 6 unmatched records

## 8. Challenges and Solutions

- Missing values: Identified and handled according to data availability.
- Duplicate records: Removed exact duplicate rows.
- Inconsistent formats: Standardized text and data types.
- Invalid values: Applied validation rules.
- Unmatched IDs: Preserved unmatched records for investigation.

## 9. Output Files

- customers_clean.csv
- products_clean.csv
- orders_clean.csv
- new_daily_batch_clean.csv
- previous_days_summary_clean.csv
- integrated_orders.csv
- unmatched_customers.csv
- unmatched_products.csv

## 10. Conclusion

The project applied data cleaning, validation, standardization, and integration techniques to prepare structured datasets for further analysis.
