# Group Health Analytics Using PySpark

A Big Data analytics project developed using PySpark to analyze student health biodata, perform data cleaning, feature engineering, risk analysis, and MongoDB integration.

##  Project Overview

This project focuses on processing and analyzing student health-related biodata using Apache Spark (PySpark). The dataset contains demographic, academic, and medical information of students such as height, weight, blood pressure, cholesterol levels, and department details.

The project demonstrates how Big Data technologies can be used for:

- Data preprocessing and cleaning
- Handling missing and invalid values
- Feature engineering
- Health risk analysis
- Data aggregation and visualization
- MongoDB integration


##  Group Members

| Student ID | Name |
|------------|------|
| CIT-23-02-0163 | Damsara Dissanayake |
| CIT-23-02-0335 | A.O.V. Jayasooriya |
| CIT-23-02-0356 | Thamindu Kavindhya |
| CIT-23-02-0176 | Tharanya Pushparaj |


##  Technologies Used

- Python
- PySpark
- Google Colab
- MongoDB Atlas
- Pandas
- Matplotlib


##  Dataset Information

The dataset contains 100 student records with 12 attributes including:

- Student ID
- Name
- Age
- Gender
- Department
- Academic Year
- Height
- Weight
- Blood Pressure
- Cholesterol Levels


##  Project Workflow

### 1️⃣ Data Loading
- Connected Google Drive with Google Colab
- Loaded CSV dataset using PySpark DataFrame

### 2️⃣ Data Cleaning & Preprocessing
- Checked schema and summary statistics
- Identified invalid values (0 values in medical columns)
- Replaced invalid values with NULL
- Applied group-wise mean imputation:
  - Height & Weight → by Gender
  - Cholesterol → by Department

### 3️⃣ Feature Engineering
Generated new analytical features such as:

- BMI Calculation
- BMI Categories
- High Blood Pressure Flag
- At-Risk Classification
- Reason for At-Risk Status

### 4️⃣ Data Analysis
Performed analytical aggregations including:

- Average BMI by Department
- Percentage of At-Risk Students
- Mean Blood Pressure by Academic Year
- Gender-wise BMI Pivot Table
- Sorted At-Risk Student Analysis

### 5️⃣ Data Visualization
Created visualizations for:
- BMI Category Distribution
- Health Risk Trends

### 6️⃣ MongoDB Integration
- Connected PySpark with MongoDB Atlas
- Uploaded cleaned data into MongoDB collection
- Retrieved and verified stored data


##  Key Findings

- Data Science (DS) department had the highest average BMI.
- DS department recorded the highest percentage of at-risk students.
- Multiple students were identified with obesity, high blood pressure, and high cholesterol.
- Feature engineering improved interpretability of health conditions.
