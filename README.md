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



 ##How It Works
Step 1: Input and File Check
Asks the user for dataset path and name

Validates the file and checks format

Step 2: Duplicate Detection
Finds and exports duplicates to {dataset_name}_duplicates.csv

Removes them from the main dataset

Step 3: Missing Value Handling
Converts numeric-looking object columns to numeric

Fills missing numeric values with the column mean

Drops rows with missing non-numeric values

Step 4: Outlier Removal (Using IQR method)
Detects outliers in numeric columns

Removes them from the dataset

Step 5: Exporting Clean Data
Final cleaned dataset is saved as {dataset_name}_Clean_data.csv

Displays a success message with the number of rows and columns






🧠 Final Thoughts
Data Cleaning Master simplifies the pre-processing stage for any data analysis or data science workflow. It’s beginner-friendly, efficient, and can save hours of manual work. Perfect for students, analysts, or professionals who frequently work with raw data.














