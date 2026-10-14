# 🎓 Mint Technologies — Clean & Structure

## 📊 Retail Sales Data Cleaning & Preprocessing

**Domain:** Data Analytics  
**Project Type:** Data Cleaning and Preprocessing  
**Tools:** Python, Pandas, NumPy, Jupyter Notebook  
**Dataset:** Retail Sales Forecasting — Kaggle (`train.csv`)

---

## 📌 Project Overview

This project focuses on cleaning and organising a retail sales dataset using Python and Pandas.

The main goal is to improve data quality and prepare the dataset for further analysis. The project includes checking missing values, identifying duplicate records, correcting date formats, standardising column names, and validating the cleaned data.

The cleaned dataset is saved as a new CSV file and can be used for Exploratory Data Analysis (EDA), sales reporting, and business analysis.

## 🎯 Objectives

- Load and inspect the raw retail sales dataset.
- Check missing values, duplicate records, and data types.
- Remove duplicate rows where present.
- Convert date columns into the correct datetime format.
- Standardise column names for consistency.
- Investigate missing values and unusual data entries.
- Apply suitable data cleaning techniques.
- Validate the dataset after cleaning.
- Save the cleaned dataset as a new CSV file.
- Prepare reliable data for further analysis and reporting.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Data cleaning and preprocessing |
| Pandas | Data manipulation and validation |
| NumPy | Numerical operations |
| Jupyter Notebook | Coding and documenting the workflow |
| CSV | Storing the raw and cleaned datasets |
| GitHub | Project documentation and version control |

## 📂 Project Directory Structure

```text
Mint-Technologies-Clean-and-Structure/
│
├── data/
│   ├── raw/
│   │   └── train.csv
│   │
│   └── cleaned/
│       └── cleaned_dataset.csv
│
├── notebooks/
│   └── 01_clean_and_structure.ipynb
│
└── README.md
```

**Folder description:**

- `data/raw/` — Contains the original dataset downloaded from Kaggle.
- `data/cleaned/` — Stores the cleaned dataset.
- `notebooks/` — Contains the Jupyter Notebook with the data cleaning steps.
- `README.md` — Explains the project, objectives, methodology, and results.

## 📊 Dataset Information

The dataset was downloaded from Kaggle.

**Dataset Source:** [Retail Sales Forecasting — Kaggle](https://www.kaggle.com/datasets/rohitsahoo/sales-forecasting)

| Attribute | Initial Finding |
|---|---|
| Input file | `train.csv` |
| Total rows | 9,800 |
| Total columns | 18 |
| Exact duplicate rows | 0 |
| Missing values | 11 |
| Column with missing values | `Postal Code` |
| Date columns | `Order Date`, `Ship Date` |
| Date conversion | Converted to datetime format |
| Column standardisation | Column names converted to lowercase |

*Note: These values are based on the initial dataset inspection. Verify them against the final notebook output before submission.*

## 🔍 Data Cleaning Methodology

### 1. Data Loading and Initial Inspection

- Imported Pandas and NumPy.
- Loaded the original `train.csv` file.
- Checked the first few rows and dataset dimensions.
- Reviewed column names and data types.
- Examined missing values and basic statistics.

### 2. Data Quality Assessment

- Checked the number of rows and columns.
- Identified missing values in each column.
- Checked for duplicate records.
- Reviewed unique values in relevant columns.
- Inspected numerical columns for unusual values.

### 3. Duplicate Detection and Removal

- Used Pandas to identify duplicate rows.
- Found zero exact duplicate rows during the initial inspection.
- Verified the duplicate count during validation.
- Avoided unnecessary deletion when no duplicates were present.

### 4. Missing Value Handling

- Identified 11 missing values in the `Postal Code` column during the initial inspection.
- Examined the missing values before deciding how to handle them.
- Avoided replacing missing values with arbitrary data.
- Applied an appropriate strategy based on the dataset's requirements.
- Checked missing-value counts after cleaning.

### 5. Date Type Conversion

- Converted `Order Date` into datetime format.
- Converted `Ship Date` into datetime format.
- Verified the resulting data types.
- Prepared the date columns for future time-based analysis.

### 6. Column Name Standardisation

- Converted column names to lowercase.
- Improved consistency and readability.
- Made column names easier to use in Python.
- Preserved the meaning of the original columns.

### 7. Data Anomaly Investigation

- Inspected numerical values for unusual entries.
- Investigated potential inconsistencies where applicable.
- Considered the business context before changing or removing values.
- Avoided deleting unusual values without a valid reason.

### 8. Data Validation

- Checked the dataset dimensions after cleaning.
- Verified the duplicate count.
- Reviewed missing-value counts.
- Confirmed the date column data types.
- Inspected the cleaned DataFrame before saving.

### 9. Exporting the Cleaned Dataset

The cleaned dataset is saved separately from the original file.

**Output file:** `cleaned_dataset.csv`

The exported CSV should be generated by running the final notebook and should match the cleaning results shown in the notebook.

## ✅ Acceptance Criteria

The project is considered complete when:

- The dataset loads successfully into Pandas.
- Duplicate rows are removed where present.
- Date columns are converted to datetime format where applicable.
- Column names and relevant text values are standardised.
- Missing values and unusual entries are investigated.
- The cleaned dataset passes validation checks.
- The cleaned CSV file is exported successfully.
- The notebook clearly documents the cleaning process.

## 📈 Expected Outcomes

This project demonstrates the ability to:

- Identify common data quality issues.
- Check and handle missing values.
- Detect duplicate records.
- Convert date columns into datetime format.
- Standardise column names.
- Investigate unusual data values.
- Validate and export cleaned data.
- Prepare datasets for further analysis.

## 💼 Business Relevance

Clean and reliable data is important for accurate retail reporting and business analysis.

Missing information, inconsistent column names, incorrect date formats, and duplicate records can affect the quality of reports and analytical results.

This project demonstrates how raw retail data can be cleaned and organised before being used for sales analysis, business reporting, and dashboard development.

## ▶️ How to Run the Project

### Step 1: Install Python and Jupyter Notebook

Ensure that Python and Jupyter Notebook are installed on your system.

### Step 2: Install the required libraries

Open Command Prompt or a terminal and run:

```bash
pip install pandas numpy matplotlib seaborn jupyter openpyxl
```

### Step 3: Place the dataset

Download the Retail Sales Forecasting dataset from Kaggle and place `train.csv` inside the `data/raw/` folder.

### Step 4: Start Jupyter Notebook

Run the following command from the project directory:

```bash
jupyter notebook
```

### Step 5: Open the notebook

Open `notebooks/01_clean_and_structure.ipynb`.

### Step 6: Run the cleaning process

Execute all notebook cells in order. Check the input and output paths if necessary.

### Step 7: Validate the results

Review the missing values, duplicate count, date data types, and final dataset dimensions.

### Step 8: Save the cleaned dataset

Confirm that `cleaned_dataset.csv` is saved in the `data/cleaned/` folder.

## 🧑‍🏫 Mentor Evaluation & Review Rubric

| Evaluation Criteria | What Is Evaluated |
|---|---|
| Data Loading | The dataset loads and is inspected correctly. |
| Data Quality Assessment | Missing values, duplicates, and data types are checked. |
| Duplicate Handling | Duplicate records are handled appropriately. |
| Date Conversion | Date columns are converted and validated. |
| Standardisation | Column names and relevant text values are consistent. |
| Missing Value Handling | Missing values are investigated and handled appropriately. |
| Anomaly Investigation | Unusual values are checked before making changes. |
| Data Validation | The cleaned dataset is checked before export. |
| Output Generation | The cleaned CSV is saved successfully. |
| Documentation | The notebook and README explain the work clearly. |
| GitHub Submission | The required files are organised properly. |

**Evaluation principle:** Cleaning decisions should be based on the dataset and its business context. Missing values and unusual entries should not be changed or removed without a valid reason.

## 📦 Required Artifacts & Deliverables

The GitHub repository should contain:

- `01_clean_and_structure.ipynb` — The completed data cleaning notebook.
- `train.csv` — The original dataset, if permitted by the dataset licence and repository limits.
- `cleaned_dataset.csv` — The cleaned dataset.
- `README.md` — The project documentation.


## 👩‍💻 Author

**Golla Bhumika**

Aspiring Data Analyst | Python | SQL | Excel | Power BI

## 🏁 Conclusion

The **Mint Technologies — Clean & Structure** project demonstrates how to clean, organise, and validate a retail sales dataset using Python and Pandas.

By checking missing values, identifying duplicates, correcting date formats, standardising column names, and validating the results, the project prepares the data for further analysis and business reporting.

**Project:** Clean & Structure  
**Organisation:** Mint Technologies  
**Milestone:** 01 — Data Cleaning and Preprocessing  
**Dataset:** Retail Sales Forecasting — Kaggle  
**Primary Tools:** Python, Pandas, Jupyter Notebook  
**Deliverables:** Data cleaning notebook and cleaned dataset
