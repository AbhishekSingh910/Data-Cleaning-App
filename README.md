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

 How It Works
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

💻 Usage
Run the script using Python:

bash
Copy
Edit
python data_cleaning_master.py
Example Interaction:

pgsql
Copy
Edit
Welcome to Data Cleaning Master!
Please enter dataset path: sample.csv
Please enter dataset name: sample1
Expected Output:

sample1_Clean_data.csv – Cleaned dataset

sample1_duplicates.csv – Duplicate records found (if any)

📊 Tested On
5+ datasets with more than 10,000 rows each

CSV and Excel formats

Datasets containing:

Missing values

Duplicates

Object type columns with numeric data

Outliers

✅ Example Output Files
File Name	Description
sample1_Clean_data.csv	Cleaned dataset output
sample1_duplicates.csv	Backup of removed duplicates
🧠 Final Thoughts
Data Cleaning Master simplifies the pre-processing stage for any data analysis or data science workflow. It’s beginner-friendly, efficient, and can save hours of manual work. Perfect for students, analysts, or professionals who frequently work with raw data.














