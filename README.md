# Duplicate Data Removal using Python & Pandas

## 📌 Project Overview

This project demonstrates how to identify and remove duplicate records from a dataset using **Python and Pandas**.

It was completed as **Task 23** of the Veda Technology AI & ML Internship. A manually created student dataset is used to detect duplicate rows, clean the data, and compare the dataset before and after cleaning.

## 🎯 Objectives

- Create a student dataset using Python.
- Identify duplicate records using Pandas.
- Count the number of duplicate rows.
- Remove duplicate records.
- Compare records before and after cleaning.
- Export the cleaned dataset into a CSV file.

## 🛠️ Technologies Used

- Python
- Pandas
- Google Colab
- Jupyter Notebook
- CSV Dataset

## 📂 Dataset Information

**Dataset:** Student Dataset

| Column | Description |
|---|---|
| Student_ID | Unique student identification number |
| Name | Student name |
| Age | Student age |
| Course | Enrolled course |
| Score | Student score |

## ⚙️ Project Workflow

### 1. Create Dataset
Created a student dataset manually using Python and saved it as a CSV file.

### 2. Identify Duplicate Records
Used the `duplicated()` function to identify repeated rows.

```python
duplicate_rows = df[df.duplicated()]
duplicate_count = df.duplicated().sum()
```

### 3. Remove Duplicate Records
Used Pandas `drop_duplicates()` to remove duplicate entries.

```python
cleaned_df = df.drop_duplicates()
```

### 4. Compare Dataset

Compared the number of records before and after removing duplicates.

```python
print("Rows Before:", len(df))
print("Rows After:", len(cleaned_df))
```

### 5. Export Cleaned Dataset

Saved the cleaned dataset as a new CSV file.

```python
cleaned_df.to_csv("Cleaned_Dataset.csv", index=False)
```

## 📊 Results

| Description | Records |
|---|---:|
| Original Records | 15 |
| Duplicate Records Found | 3 |
| Duplicate Records Removed | 3 |
| Records After Cleaning | 12 |
| Remaining Duplicates | 0 |

**Result:** Successfully removed all 3 duplicate records and obtained a clean dataset containing 12 unique records.

## 📁 Project Structure

```text
Duplicate-Data-Removal/
│
├── Duplicate_Data_Removal.ipynb
├── duplicate_data.csv
├── Cleaned_Dataset.csv
└── README.md
```

## 🚀 How to Run the Project

1. Clone this repository:

```bash
git clone https://github.com/satya77713/Duplicate-Data-Removal.git
```

2. Navigate to the project folder:

```bash
cd Duplicate-Data-Removal
```

3. Install Pandas:

```bash
pip install pandas
```

4. Open the Jupyter Notebook:

```bash
jupyter notebook Duplicate_Data_Removal.ipynb
```

5. Run all notebook cells.
6. Check the duplicate records and cleaned CSV output.

Alternatively, open the notebook using Google Colab.

## 📚 Key Learnings

- Data cleaning with Python.
- Working with CSV datasets.
- Identifying duplicate records.
- Using Pandas `duplicated()` and `drop_duplicates()`.
- Exporting cleaned datasets.
- Understanding the importance of data quality in Data Analysis and Machine Learning.

## 🎓 Internship Details

- **Organization:** Veda Technology
- **Program:** AI & ML Internship
- **Task Number:** 23
- **Project:** Duplicate Data Removal

## 👨‍💻 Author

**Satya**

GitHub: [@satya77713](https://github.com/satya77713)

## 📝 Conclusion

This project provided practical experience in data preprocessing and data cleaning using Python and Pandas. By identifying and removing duplicate records, the dataset became more accurate and reliable for further data analysis and machine learning applications.

---
⭐ If you find this project useful, feel free to star the repository!
