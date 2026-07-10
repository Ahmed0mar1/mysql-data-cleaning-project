# SQL Data Cleaning Project – World Layoffs Dataset

## Overview

This project demonstrates a complete SQL data cleaning workflow using MySQL on the World Layoffs dataset from Kaggle.

The objective is to transform raw data into a clean and analysis-ready dataset by applying common data cleaning techniques used in real-world analytics projects.

---

## Dataset

Source:
https://www.kaggle.com/datasets/swaptr/layoffs-2022

---

## Objectives

The project follows a structured data cleaning process:

- Create a staging table
- Identify and remove duplicate records
- Standardize inconsistent values
- Handle missing values
- Convert data types
- Remove unnecessary rows and columns
- Produce a clean dataset ready for analysis

---

## Technologies Used

- MySQL 8+
- SQL
- Window Functions
- Common Table Expressions (CTEs)

---

## Data Cleaning Process

### 1. Create a Staging Table

The original dataset is preserved by creating a staging table for all cleaning operations.

---

### 2. Remove Duplicates

Duplicate records are identified using:

- ROW_NUMBER()
- PARTITION BY

Duplicate rows are removed while preserving the first occurrence.

---

### 3. Standardize Data

Several inconsistencies are corrected:

- Remove leading/trailing spaces
- Standardize Crypto industry names
- Remove trailing periods from country names
- Convert text dates into DATE format

---

### 4. Handle Missing Values

Missing industry values are populated using records from the same company whenever possible.

Blank values are converted into NULL for consistency.

---

### 5. Remove Unnecessary Data

Rows containing no layoff information are removed.

Temporary helper columns are dropped after cleaning.

---

## SQL Concepts Demonstrated

- Window Functions
- ROW_NUMBER()
- CTEs
- JOIN
- UPDATE
- DELETE
- ALTER TABLE
- Data Type Conversion
- NULL Handling
- String Functions
- Date Functions

---



---

## Skills Demonstrated

- SQL Data Cleaning
- Data Wrangling
- Data Preparation
- Database Management
- Analytical Thinking
- Query Optimization
- Data Quality

---


