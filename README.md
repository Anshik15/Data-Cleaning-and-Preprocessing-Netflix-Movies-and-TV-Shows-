etflix-Movies-and-TV-Shows Dataset Cleaning Project

Objective
The goal of this project was to clean and prepare a raw Netflix dataset by handling missing values, correcting data types, standardizing formats, and ensuring consistency across the data for further analysis or modeling.

Tools Used
Python (Pandas)
Jupyter Notebook
Visual Studio Code

Dataset Overview
The dataset contains information about Netflix Movies and TV Shows, with columns such as:

show_id
type
title
director
cast
country
date_added
release_year
rating
duration
listed_in
description

Data Cleaning Steps
1. Missing Value Handling
Filled missing director with "Unknown".
Filled missing cast with "Not Available".
Filled missing country with the most frequent value (mode).
Filled missing rating with "Not Rated".
2.Dropped rows with missing date_added and duration.
3. Duplicate Handling
Checked for duplicates using df.duplicated().sum() → No duplicates found.
4. Standardization
Column names converted to lowercase with underscores.
Stripped whitespace and standardized casing for columns like type, country, rating, etc.
5. Date Format Handling
Converted date_added to datetime format.
Created a formatted date string column: date_added_ddmmyyyy (in dd-mm-yyyy format).
6. Data Type Corrections
Ensured release_year is of type int.
Ensured duration is treated as a str.
7. Feature Engineering
Extracted numeric part of duration into duration_num.
Extracted time unit (e.g., "min", "season") into duration_type.

Final Outcome
Cleaned, structured, and well-prepared dataset that is ready to use for further analysis.
Ready for EDA, visualization, and machine learning tasks.
Deliverables
Cleaned dataset (CSV/Excel)

Conclusion
This project demonstrates fundamental data preprocessing steps required for real-world datasets. By resolving inconsistencies, handling nulls, and engineering useful features, the dataset is now in excellent shape for insights and predictive modeling.
