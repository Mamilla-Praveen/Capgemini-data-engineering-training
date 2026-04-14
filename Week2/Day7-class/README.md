# 🚀 Day 7 – Databricks & PySpark Learning

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![PySpark](https://img.shields.io/badge/PySpark-Big%20Data-orange?logo=apachespark)
![Databricks](https://img.shields.io/badge/Databricks-Platform-red?logo=databricks)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Overview

This session focused on core concepts of PySpark and Databricks, including data transformations, storage formats, widgets, and real-world data engineering practices.

---

## 🧠 1. User Defined Functions (UDF)

* UDF allows creation of custom logic in PySpark
* Converts Python functions into distributed Spark functions

### ✅ Key Points

* Used when built-in functions are not sufficient
* Requires return type (e.g., `StringType`)
* Applied on DataFrame columns

---

## 💾 2. Writing Data in PySpark

```python
df.write.mode("overwrite").parquet("path")
```

### ✅ Key Points

* `write` → saves DataFrame
* `overwrite` → replaces existing data
* Supports multiple formats (Parquet, CSV, JSON)

---

## 📦 3. Parquet File Format

* Columnar storage format
* Optimized for big data processing

### ✅ Advantages

* Faster query performance
* Compression reduces storage
* Reads only required columns

---

## 🎛️ 4. Databricks Widgets

### Types of Widgets

* 🔹 Combobox → select or type
* 🔹 Dropdown → select only
* 🔹 Multiselect → multiple selections
* 🔹 Textbox → user input

### Example

```python
dbutils.widgets.get("widget_name")
```

---

## 🔄 5. Full Load vs Incremental Load

### 🔹 Full Load

* Loads entire dataset every time
* Simple but resource-intensive

### 🔹 Incremental Load

* Loads only new/updated data
* Efficient and faster

---

## 🔗 6. End-to-End Data Pipeline

### Pipeline Flow:

1. 📥 Data Ingestion
2. 🧹 Data Cleaning
3. 🔄 Transformation
4. 💾 Storage
5. 📊 Analysis

---

## 🏆 Key Learnings

* Distributed data processing using PySpark
* Efficient storage with Parquet
* Dynamic inputs using widgets
* Real-world pipeline design concepts

---

## 📈 Future Improvements

* Implement real-time streaming pipeline
* Use Delta Lake for advanced operations
* Add dashboard integration (Power BI / Tableau)


---

## 🙌 Conclusion

Today practice strengthened understanding of data engineering fundamentals and practical implementation of PySpark workflows in Databricks.

---

