# Task 23: Duplicate Data Removal using Pandas

## Overview

This project is part of the Veda Technology AI & ML Internship.

The objective of this task is to identify duplicate records in a dataset and remove them using Python and Pandas.

A manually created student dataset is used to demonstrate duplicate detection, data cleaning, and comparison of dataset sizes before and after removing duplicates.

## Objective

- Identify duplicate records in a dataset.
- Calculate the number of duplicate rows.
- Remove duplicate records using Pandas.
- Compare row counts before and after cleaning.
- Understand the importance of data cleaning before analysis and machine learning.

## Dataset Information

- **Dataset:** Student Dataset
- **File:** `duplicate_data.csv`
- **Total Records Before Cleaning:** 15
- **Total Columns:** 5
- **Duplicate Records:** 3

### Dataset Columns

| Column | Description |
|---|---|
| Student_ID | Unique student identification number |
| Name | Student name |
| Age | Student age |
| Course | Enrolled course |
| Score | Student score |

## Tools & Technologies

- Python
- Pandas
- Google Colab
- Jupyter Notebook

## Operations Performed

### 1. Create the Dataset

A student dataset was manually created using Python and saved as a CSV file.

```python
df.to_csv("duplicate_data.csv", index=False)
```

### 2. Identify Duplicate Records

Used the Pandas `duplicated()` method to identify repeated rows.

```python
duplicate_rows = df[df.duplicated()]

duplicate_count = df.duplicated().sum()
```

**Result:** 3 duplicate records were identified.

### 3. Remove Duplicate Records

Used `drop_duplicates()` to remove repeated rows.

```python
cleaned_df = df.drop_duplicates()
```

### 4. Compare Before and After Cleaning

Compared the dataset row counts before and after removing duplicates.

```python
print("Rows Before:", len(df))
print("Rows After:", len(cleaned_df))
```

### 5. Save the Cleaned Dataset

Exported the cleaned DataFrame as a CSV file.

```python
cleaned_df.to_csv("Cleaned_Dataset.csv", index=False)
```

## Results

| Description | Records |
|---|---:|
| Original records | 15 |
| Duplicate records found | 3 |
| Duplicate records removed | 3 |
| Records after cleaning | 12 |
| Remaining duplicates | 0 |

## Key Concepts Learned

- Creating CSV datasets using Pandas.
- Identifying duplicate rows using `duplicated()`.
- Counting duplicate records.
- Removing duplicates using `drop_duplicates()`.
- Comparing dataset sizes before and after cleaning.
- Exporting cleaned data using `to_csv()`.

## Project Structure

```text
Duplicate-Data-Removal/
│
├── Duplicate_Data_Removal.ipynb
├── duplicate_data.csv
├── Cleaned_Dataset.csv
└── README.md
```

## How to Run

1. Clone or download this repository.
2. Open `Duplicate_Data_Removal.ipynb` in Google Colab.
3. Run the notebook cells in order.
4. The student dataset will be created and saved as a CSV file.
5. Execute the duplicate detection and removal operations.
6. View the cleaned dataset and compare the before-and-after row counts.

## Internship Details

- **Organization:** Veda Technology
- **Track:** AI & ML Internship
- **Task:** 23 – Duplicate Data Removal

## Conclusion

Successfully completed duplicate data removal using Python and Pandas. This task provided practical experience in identifying repeated records, cleaning datasets, and improving data quality for further analysis and machine learning applications.
