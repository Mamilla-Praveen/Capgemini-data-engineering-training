# Phase 4 – Bucketing & Segmentation in PySpark

## Topics Covered
Concept of bucketing (segmentation)
Converting continuous data into categories (Gold, Silver, Bronze)
Multiple segmentation methods in PySpark:
- Conditional logic using when()
- SQL CASE statement
- Bucketizer (MLlib)
- Quantile-based segmentation using approxQuantile()
- Window-based ranking using percent_rank()

## Objective
The objective of this phase is to understand how to transform continuous numerical data into meaningful categories using different segmentation techniques. This helps in simplifying analysis and making data more interpretable for business decisions.

## Approach
- Loaded dataset into PySpark DataFrame
- Analyzed distribution of numerical columns
- Applied different segmentation techniques
- Compared results of rule-based and data-driven approaches
- Converted segmented outputs into meaningful business labels

## Methods Practiced

### Rule-Based Segmentation
- Used fixed thresholds to classify data into categories
- Implemented using when() and SQL CASE statements

### Quantile-Based Segmentation
- Used approxQuantile() to divide data into equal-sized groups

### Bucketizer (MLlib)
- Converted continuous values into predefined buckets

### Window-Based Segmentation
- Used percent_rank() with window functions

## Key Transformations Used
- when()
- approxQuantile()
- Bucketizer
- percent_rank()
- groupBy()

## Conceptual Understanding
- Bucketing simplifies continuous data
- Rule-based vs data-driven segmentation difference

## Output / Results
- Segmented dataset (Gold, Silver, Bronze)
- Distribution analysis

## Learnings
- Importance of segmentation
- Practical PySpark usage

## Conclusion
Phase 4 focused on converting raw data into meaningful segments for better analysis.
