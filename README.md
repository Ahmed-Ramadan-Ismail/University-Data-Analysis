# 🎓 University Data Analysis

> **End-to-End Data Analysis & Data Modeling Project**  
> From raw Kaggle data to SQL analysis, Python data cleaning, Star Schema modeling, and Power BI insights.

---

## 📌 Project Overview

This project is an end-to-end **University Data Analysis** solution built to transform raw university data into a clean, structured, and analysis-ready data model.

The project follows a complete analytical workflow:

**Kaggle Dataset → Business Questions → SQL Analysis → One Big Table → Python Data Cleaning → Star Schema → Power BI**

The main goal is not only to build a dashboard, but to demonstrate the full journey of the data from its original source to the final analytical model.

---

## 🔄 End-to-End Data Pipeline

<p align="center">
  <img src="assets/university-data-analysis-pipeline.png" alt="University Data Analysis End-to-End Pipeline" width="100%">
</p>

### Pipeline Steps

| Step | Stage | Description |
|---|---|---|
| 1 | **Data Source** | University dataset collected from Kaggle |
| 2 | **Business Questions** | Defined 10 business/analytical questions to guide the analysis |
| 3 | **SQL Analysis** | Used SQL Server queries to answer the business questions |
| 4 | **One Big Table** | Combined the required university information into one analytical table |
| 5 | **Python Data Cleaning** | Loaded the Excel data with Python and performed cleaning, validation, and transformation |
| 6 | **Star Schema** | Converted the cleaned One Big Table into a dimensional model |
| 7 | **Power BI** | Built the final data model, measures, analysis, and interactive dashboard |

---

## 🎯 Business Questions

Before building the final data model, the project started with **10 business questions**.

These questions were used to determine:

- What information should be analyzed?
- Which columns are required?
- Which metrics should be calculated?
- What relationships exist between students, courses, faculty, and enrollment?
- Which insights should eventually appear in the dashboard?

The questions were answered using **SQL Server** before moving to the data-cleaning and modeling stages.

---

## 🗄️ SQL Analysis

SQL Server was used as an analytical layer to query the university data and answer the defined business questions.

The SQL analysis focused on areas such as:

- Student enrollment
- Academic performance
- Courses
- Departments
- Faculty
- Academic years
- Semesters
- Enrollment status
- Grades and scores

The SQL queries are included in the project files.

---

## 📊 One Big Table

After the SQL analysis, the required information was combined into a **One Big Table**.

The table contains **8,000 enrollment records** and **38 data columns**.

The main areas represented in the table include:

### Student Information
- Student ID
- Student Number
- Student Name
- Email
- Gender
- Date of Birth
- Student Enrollment Date
- Expected Graduation
- Student Status
- GPA

### Department Information
- Department ID
- Department Code
- Department Name

### Course Information
- Course ID
- Course Code
- Course Title
- Credits
- Course Level

### Faculty Information
- Faculty ID
- Faculty Name
- Faculty Email
- Faculty Rank

### Section Information
- Section ID
- Section Number
- Delivery Method
- Section Status

### Semester Information
- Semester ID
- Term
- Academic Year
- Semester Name
- Semester Start Date
- Semester End Date

### Enrollment & Performance
- Enrollment ID
- Enrollment Date
- Enrollment Status
- Final Grade
- Final Score

---

## 📥 Excel Data Layer

The One Big Table was loaded into **Excel** from SQL Server.

This Excel file was then used as the input for the Python data-cleaning stage.

The workflow was:

```text
SQL Server
    ↓
Get Data
    ↓
Excel
    ↓
One Big Table
```

---

## 🐍 Python Data Cleaning

Python was used to read the Excel One Big Table and prepare the data for dimensional modeling.

The cleaning process included tasks such as:

- Detecting missing values
- Checking duplicate records
- Validating data types
- Checking inconsistent values
- Handling invalid data
- Standardizing fields
- Preparing columns for dimensional modeling
- Validating the final dataset before loading it into Power BI

Main Python libraries used:

```text
Python
Pandas
NumPy
OpenPyXL
```

---

## ⭐ Star Schema

After cleaning the One Big Table, the data was transformed into a **Star Schema**.

The final model contains one central fact table surrounded by dimension tables.

### Fact Table

**FactEnrollment**

Contains measurable enrollment and academic performance information.

Examples:

- Enrollment ID
- Student ID
- Course ID
- Faculty ID
- Semester ID
- Final Score
- Final Grade
- Enrollment Status

### Dimension Tables

**Dim_students**

Contains student-related descriptive information.

**DimCourse**

Contains course-related information.

**DimFaculty**

Contains faculty-related information.

**Dim_Date**

Contains date attributes used for time-based analysis.

Examples:

- Date
- Day Number
- Month Name
- Month Number
- Year

### Model Structure

```text
                  Dim_students
                       |
                       |
DimCourse ---- FactEnrollment ---- DimFaculty
                       |
                       |
                    Dim_Date
```

---

## 📈 Power BI

The final Star Schema was imported into **Power BI** to create the analytical model and dashboard.

The Power BI stage includes:

- Data model
- Relationships
- DAX measures
- KPIs
- Academic analysis
- Student analysis
- Enrollment analysis
- Time-based analysis
- Interactive visualizations

The dashboard is designed to turn the cleaned university data into meaningful business and academic insights.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **Kaggle** | Data Source |
| **SQL Server** | SQL analysis and data preparation |
| **Excel** | One Big Table data layer |
| **Python** | Data cleaning and transformation |
| **Pandas** | Data manipulation |
| **NumPy** | Numerical processing |
| **Power BI** | Data modeling, DAX, visualization |
| **Star Schema** | Dimensional data modeling |

---

## 📁 Project Structure

```text
University-Data-Analysis/
│
├── README.md
│
├── assets/
│   └── university-data-analysis-pipeline.png
│
├── data/
│   └── one_big_table.xlsx
│
├── sql/
│   └── business_questions.sql
│
├── python/
│   └── data_cleaning.py
│
├── powerbi/
│   └── university_data_analysis.pbix
│
└── docs/
    └── data_model.png
```

> File names can be adjusted to match the final GitHub repository structure.

---

## 🔍 Project Workflow

```text
Raw Kaggle Data
       ↓
Define 10 Business Questions
       ↓
SQL Server Analysis
       ↓
Exploratory Data Analysis
       ↓
One Big Table
       ↓
Excel
       ↓
Python Data Cleaning
       ↓
Clean Data
       ↓
Star Schema
       ↓
Power BI Data Model
       ↓
Dashboard & Insights
```

---

## 📌 Key Learning Outcomes

Through this project, I practiced:

- Translating business requirements into analytical questions
- Writing SQL queries for data analysis
- Performing exploratory data analysis
- Working with One Big Table structures
- Cleaning and validating data using Python
- Designing a Star Schema
- Creating fact and dimension tables
- Building date dimensions
- Creating relationships in Power BI
- Developing analytical dashboards
- Turning raw data into actionable insights

---

## 👨‍💻 Project Goal

This project demonstrates an end-to-end approach to **Data Analysis and Data Engineering**, combining:

**SQL + Python + Data Cleaning + Data Modeling + Power BI**

The objective is to show how raw university data can be transformed into a structured analytical solution suitable for reporting and decision-making.

---

## 📬 Contact

**Ahmed Ramadan**

- GitHub: [Add your GitHub profile]
- LinkedIn: [Add your LinkedIn profile]
- Email: [Add your email]

---

⭐ If you find this project useful, feel free to star the repository.
