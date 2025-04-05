# 🧹 Data Cleaning Master

**Data Cleaning Master** is a Python-based application designed to clean messy datasets quickly and efficiently. It handles common issues like duplicate records, missing values, and incorrect data types, and provides a cleaned version of your dataset along with a backup of duplicates.

---

## 🚀 Features

- Supports **CSV** and **Excel** file formats
- Automatically detects and removes **duplicate records**
- Handles **missing values**:
  - Fills missing numeric values with column mean
  - Drops rows with missing non-numeric values
- Converts numeric-looking **object type columns** to proper `int` or `float`
- Saves both **cleaned data** and **duplicate backup**
- Works on **large datasets** (tested on 10k+ rows)
- Provides clear, user-friendly prompts during the process

---

## 📌 Objectives

- Load and clean datasets in `.csv` or `.xlsx` format
- Identify and export duplicate records
- Handle missing values effectively
- Perform intelligent data type conversions before processing
- Save the cleaned dataset with a new file name

---

## 🛠️ Requirements

- Python 3.x
- pandas
- numpy
- openpyxl
- xlrd

Install the required libraries using:

```bash
pip install pandas numpy openpyxl xlrd














