# CSV Filehandling and Manipulation

This repository contains the deliverables for the **Sunday Project (Data Quality, Insights & CSV Operations)** as part of the AI Engineering Bootcamp (Module 02).

## GitHub Repository Link
- **Repository URL:** https://github.com/Humam-hub/CSV-File-Handling-and-Manipulation

---

## Project Overview

The project is split into two logical parts executed sequentially within a single runnable Google Colab / Jupyter Notebook:

### Part A: Data Quality & Basic Insights (70 Marks)
- **Objectives:** 
  - Load and inspect the raw sales dataset (`sales_raw.csv`).
  - Clean the dataset (handling duplicates, missing values, standardizing columns, and correcting incorrect records).
  - Create a new calculated metric: `revenue` (`quantity` * `unit_price`).
  - Perform visual EDA (exploratory data analysis) using charts.
  - Export the clean results to `cleaned_sales.csv`.

### Part B: CSV File Handling & Manipulation (30 Marks)
- **Objectives:**
  - Read the `cleaned_sales.csv` produced in Part A.
  - Add a computed `tax_amount` column (5% of `revenue`).
  - Target and update **Books** items, increasing their `unit_price` by 10% using `.loc[]` and recalculating dependent columns.
  - Drop a transaction row by ID and handle temporary operational columns.
  - Save the final manipulation as `sales_updated.csv` and verify the integrity.

---

## How to Run the Notebook

### 1. Requirements & Prerequisites
You will need the following libraries installed in your Python environment:
- `pandas`
- `numpy`
- `matplotlib` (if plotting charts in Part A)
- `seaborn` (if plotting charts in Part A)
- `pypdf` (for PDF brief parsing)

### 2. File Structure
Ensure the following structure is maintained in your directory/workspace:
```text
├── cleaned_sales.csv                   # Output generated from Part A
├── sales_updated.csv                   # Output generated from Part B
├── CSV File Handling and Manipulation.ipynb
└── README.md                           # This instructions and metadata file
```

### 3. Execution Steps
1. Open the `.ipynb` notebook file in Google Colab or your local Jupyter instance.
2. Ensure `sales_raw.csv` and `Sunday_Project_Brief_100_Marks.pdf` are loaded into your working directory (e.g. `/content/` inside Google Colab).
3. Execute the code cells sequentially from top to bottom.
4. Confirm that the terminal outputs print the step summaries, and that `cleaned_sales.csv` and `sales_updated.csv` are generated correctly.
