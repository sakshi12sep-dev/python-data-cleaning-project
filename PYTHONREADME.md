# 🐍 Python Data Cleaning & Inspection Project (using Pandas)

## 📋 Project Overview
This project demonstrates how to **inspect, clean, and prepare raw data** for analysis using Python’s **pandas** library.  
It focuses on identifying and fixing common data quality issues such as missing values, duplicates, inconsistent entries, incorrect data types, and outliers — all crucial steps in the data preprocessing stage.

---

## 🎯 Objectives
- Load and inspect raw data  
- Detect and handle missing values  
- Remove or consolidate duplicate records  
- Identify and correct data inconsistencies  
- Convert incorrect data types  
- Detect and treat outliers appropriately  

---

## 🧰 Tools & Technologies Used
- **Python** 🐍  
- **Pandas** (for data manipulation)  
- **NumPy** (for numerical operations)  
- **Jupyter Notebook** (for step-by-step execution and visualization)

---

## 📊 Steps Performed

### 1️⃣ Data Inspection
- Checked data shape, column names, and data types using `info()`, `dtypes`, and `describe()`.
- Identified potential issues such as missing or inconsistent data.

### 2️⃣ Handling Missing Data
- Used `isnull()` and `sum()` to locate missing values.  
- Applied appropriate strategies:
  - Dropping rows or columns with excessive missing data using `dropna()`.  
  - Filling missing data with mean, median, or mode using `fillna()`.  

### 3️⃣ Handling Duplicates
- Identified duplicate rows using `duplicated()`.  
- Removed them with `drop_duplicates()`.

### 4️⃣ Fixing Inconsistencies
- Cleaned inconsistent categorical entries (e.g., capitalization, spelling differences).  
- Standardized text formats using string methods like `str.lower()`, `str.strip()`, and `replace()`.

### 5️⃣ Correcting Data Types
- Converted incorrect data types using `astype()`.  
- Ensured numerical columns were properly formatted for mathematical operations.

### 6️⃣ Handling Outliers
- Detected outliers using statistical methods (IQR, Z-score).  
- Treated them by capping, transforming, or removing depending on context.

---

## 🧾 Example Commands
```python
df.info()
df.isnull().sum()
df.drop_duplicates(inplace=True)
df['Age'].fillna(df['Age'].median(), inplace=True)
df['Category'] = df['Category'].str.lower().str.strip()
