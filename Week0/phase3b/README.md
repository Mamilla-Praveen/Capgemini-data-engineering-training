# Phase – Data Cleaning Using PySpark

## Objective
In this phase, the goal is to work with messy data and apply data cleaning techniques using PySpark. This ensures the dataset is reliable before performing any further processing or analysis.

## Problem Summary
We were given a dataset containing multiple data quality issues such as missing values, duplicate records, and invalid entries.

The task was to:

Identify data quality issues
Clean the dataset
Validate the cleaned data
Perform basic aggregation

## Approach

Loaded the dataset into a PySpark DataFrame
Identified data issues such as null values, duplicates, and invalid data

### Data Cleaning Steps

Removed records with missing key values
Handled null values in important columns
Removed duplicate records
Filtered out invalid data
Validated the cleaned dataset by comparing before and after results
Performed aggregation to derive insights

## Key Transformations Used

dropna() → to handle missing values
dropDuplicates() → to remove duplicate records
filter() → to remove invalid data
groupBy() → for aggregation

## Output / Results
The following outputs were generated:

Cleaned dataset with no invalid or duplicate records
Aggregated data showing distribution across categories

Screenshots of outputs are available in the outputs/ folder.

## Data Engineering Considerations

Removed invalid and inconsistent data to improve accuracy
Ensured no duplicate records affect results
Validated cleaned data before performing aggregation

## Challenges Faced

Handling multiple types of data issues in a single dataset
Deciding how to treat missing values without losing important data

## Learnings

Importance of data cleaning in real-world scenarios
Techniques to handle missing and invalid data
How poor data quality impacts final results
