# VEDA Technology – Missing Value Identification

## Introduction

This project was completed as part of a Data Analytics task for VEDA Technology.

The objective of this project is to identify missing values in a dataset, calculate their percentages, summarize the results, visualize missing data, and document the key findings.

The analysis was performed using Python, Pandas, Matplotlib, and Jupyter Notebook.

## Dataset

This project uses the Titanic Dataset.

The dataset contains passenger information including:

- Passenger ID
- Survival status
- Passenger class
- Name
- Gender
- Age
- Siblings/Spouses
- Parents/Children
- Ticket
- Fare
- Cabin
- Embarked Port

## Objectives

The main objectives of this task are:

1. Load and inspect the dataset.
2. Identify columns containing missing values.
3. Calculate the number of missing values.
4. Calculate the percentage of missing values.
5. Create a missing-value summary.
6. Visualize missing values using a bar chart.
7. Document the key findings.
8. Understand why missing values should not be deleted blindly.

## Analysis Performed

### 1. Dataset Loading

The Titanic dataset was loaded using Pandas.

### 2. Dataset Inspection

The dataset was inspected to understand its shape, columns, and data types.

### 3. Missing Value Identification

Missing values were identified using Pandas `isnull()` and `sum()` functions.

### 4. Missing Value Summary

The number and percentage of missing values were calculated for each column containing missing data.

The summary was saved as:

`missing_value_summary.csv`

### 5. Missing Value Visualization

A bar chart was created using Matplotlib to visualize the number of missing values in each affected column.

## Key Findings

The analysis identified missing values in the following columns:

| Column | Missing Values |
|---|---:|
| Age | 177 |
| Cabin | 687 |
| Embarked | 2 |

### Observations

- The `Cabin` column contains the highest number of missing values.
- The `Age` column also contains a significant number of missing values.
- The `Embarked` column contains only a small number of missing values.
- Missing data should be handled according to the column, amount of missingness, and purpose of the analysis.
- Rows should not be deleted blindly because this can reduce the dataset and potentially remove useful information.

## Technologies Used

- Python
- Pandas
- Matplotlib
- Jupyter Notebook

## Project Structure

```text
veda-technology-task-12-missing-value-identification/
│
├── Titanic-Dataset.csv
├── Missing_Value_Identification.ipynb
├── missing_value_summary.csv
└── README.md
