# Phase 3A – Data Cleaning using PySpark

## Objective
The objective of this phase is to perform data cleaning on a dataset using PySpark. This includes identifying null values, duplicate records, and invalid data, and transforming the dataset into a clean and usable format.

## Problem Summary
In this phase, I worked with a customer dataset containing the following fields:
- customer_id
- name
- city
- age

The dataset contained:
- Null values in multiple columns
- Duplicate records
- Invalid values such as negative age

The main tasks were:
- Identify data quality issues
- Clean and transform the dataset
- Generate a final cleaned dataset for analysis

## Approach
The following steps were followed to complete the task:

- Created a PySpark DataFrame using sample data

- Identified data issues:
  - Filtered rows with null values
  - Detected duplicate records using groupBy()
  - Identified invalid age values (age < 0)

- Applied data cleaning steps:
  - Removed rows where customer_id is null
  - Replaced null values in name and city with "Unknown"
  - Removed duplicate records using dropDuplicates()
  - Filtered out invalid age values

- Generated final cleaned dataset

- Performed aggregation:
  - Calculated city-wise customer count

## Key Transformations Used
- filter() → To identify and remove invalid or null records
- fillna() → To replace null values
- dropDuplicates() → To remove duplicate rows
- groupBy() → To perform aggregation
- count() → To calculate totals

## SQL Conversion
The same data cleaning logic can be implemented using SQL by:
- Identifying null values using conditions
- Detecting duplicates using GROUP BY and HAVING
- Replacing null values using COALESCE
- Removing duplicates using DISTINCT
- Filtering invalid data using WHERE clause
- Performing aggregation using GROUP BY

## Output / Results
The following outputs were generated:
- Dataset with null values identified
- Duplicate records identified
- Invalid age records filtered
- Final cleaned dataset
- City-wise customer count

## Data Engineering Considerations
- Removed null values to improve data quality
- Ensured duplicates were eliminated to avoid incorrect results
- Filtered invalid data such as negative age
- Verified row counts before and after cleaning

## Challenges Faced
- Handling multiple data quality issues in a single dataset
- Ensuring transformations were applied in correct order
- Understanding how PySpark operations translate to SQL

## Learnings
- Learned how to clean data using PySpark
- Understood handling of null values and duplicates
- Gained experience in converting PySpark logic into SQL
- Improved understanding of real-world data preprocessing

## Files in this Folder
- pyspark_code3a.py → PySpark data cleaning implementation
- outputs3a/ → Output screenshots

## Conclusion
This phase helped me understand the importance of data cleaning in data engineering. It strengthened my ability to handle real-world datasets and improved my data preprocessing skills.
