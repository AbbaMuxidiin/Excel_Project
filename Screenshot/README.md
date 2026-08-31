Student Enrollment Management & Analytics Dashboard

📊 Project Overview

This project is a Student Enrollment Management & Analytics Dashboard developed in Microsoft Excel.

The project focuses on analyzing student enrollment data and transforming raw data into meaningful insights using:

Data Cleaning

Data Quality Analysis

Pivot Tables

Pivot Charts

KPIs

Interactive Slicers

Dashboard Design

Tuition and Enrollment Analysis

The dashboard provides a clear overview of student enrollment, enrollment status, study mode, gender, academic programs, enrollment dates, and tuition fees.

🎯 Project Objectives

The main objectives of this project are to:

Identify the total number of students.

Analyze student enrollment status.

Compare students by gender.

Analyze different study modes.

Identify student distribution across academic programs.

Analyze tuition fees by program.

Analyze enrollment trends by date.

Identify missing, duplicate, invalid, and inconsistent data.

Build an interactive Excel dashboard for decision-making.

🧹 Data Cleaning & Data Quality Analysis

The data analysis identified several data-quality issues that should be addressed before the final analysis.

Gender

Gender

Count

Male

148

Female

136

Blank

15

Non-value

1

Total

300

There are blank and invalid gender values that should be reviewed during the data-cleaning stage.

Program Data Quality

The dataset contains both standardized program names and inconsistent values.

Examples of inconsistent values include:

BA

CS

NULL

Unknown

blank

non_program

Standard program names include:

Business Administration

Computer Science

Data Science

Economics

Engineering

Public Health

Recommended cleaning:

BA → Business Administration

CS → Computer Science

Review NULL, Unknown, and blank values.

Review non_program and determine whether it should remain as a category or be treated as missing data.

Study Mode Data Quality

The Study Mode field contains:

Full-Time

Part-Time

Online

N/A

NULL

Blank

non_stady_mode

The value non_stady_mode appears to be an inconsistent or misspelled category and should be reviewed.

Study Mode Summary

Study Mode

Students

Full-Time

162

Part-Time

59

Online

60

non_stady_mode

19

Total

300

Key Insight: Full-Time students represent the largest study-mode category.

Enrollment Status Data Quality

The Enrollment Status field contains:

Active

Deferred

Graduated

Withdrawn

N/A

Blank

non_status

The inconsistent and missing values should be standardized before final reporting.

Duplicate Student IDs

The analysis identified several Student IDs appearing more than once.

Examples include Student IDs with a count of 2.

These records should be reviewed to determine whether they are:

Genuine duplicate records, or

Valid multiple enrollment records for the same student.

Missing Student IDs

Some records have missing Student IDs.

Because Student_ID is an important identifier, missing values should be reviewed and corrected where possible.

📌 Pivot Tables & Analysis

1. Enrollment Status

The Enrollment Status Pivot Table shows:

Enrollment Status

Students

Active

175

Deferred

27

Graduated

64

Withdrawn

16

Total shown in Pivot

282

A Pivot Chart was created to visualize the enrollment-status distribution.

Key Insight

Active students represent the largest group, while Deferred and Withdrawn represent smaller groups.

Note: The overall dataset contains 300 records, but this Pivot Table counts Tuition_Fee. Therefore, the Pivot Total is 282 because records with missing Tuition_Fee values are excluded from this count.

2. Enrollment Date Analysis

Enrollment Date was analyzed using a Pivot Table and Line Chart.

The chart shows enrollment counts including:

18

26

23

34

20

6

10

55

78

30

However, #VALUE! appears in the Pivot Table/chart.

Enrollment Date Issue

The #VALUE! indicates that some Enrollment Date values may not be stored as valid Excel dates.

Recommended Fix

Check all Enrollment Date values.

Identify invalid or text-based dates.

Convert valid values to Excel Date format.

Correct or remove invalid dates.

Refresh the Pivot Table.

Group the dates by Month and/or Year.

3. Study Mode

The Study Mode Pivot Table contains:

Study Mode

Students

Full-Time

162

Part-Time

59

Online

60

non_stady_mode

19

Total

300

A Pie Chart was created to visualize the Study Mode distribution.

Key Insight

Full-Time is the most common study mode, followed by Online and Part-Time.

The non_stady_mode category should be reviewed during data cleaning.

4. Tuition by Program

Tuition was analyzed by academic program.

Program

Tuition

Business Administration

$36,617.50

Computer Science

$68,526.92

Data Science

$65,662.73

Economics

$19,402.25

Engineering

$42,936.93

non_program

$17,318.41

Public Health

$30,457.95

Total

$280,922.69

Key Insights

Computer Science has the highest total tuition at $68,526.92.

Data Science has the second-highest total tuition at $65,662.73.

Economics has the lowest tuition among the named standard programs.

The total tuition shown in the Pivot Table is $280,922.69.

📈 Dashboard

The final dashboard combines KPIs, charts, and interactive slicers.

Main KPIs

The dashboard includes the following key metrics:

KPI

Value

Total Students

300

Active Students

175

Graduated Students

64

Total Tuition

$280,922.69

Average Tuition

$996.18

⚠️ KPI Correction

The dashboard screenshot shows $996.18 under both Total Tuition and Average Tuition.

This is incorrect.

The correct values are:

Total Tuition

$280,922.69

Average Tuition

$996.18

The Average Tuition is approximately:

$280,922.69 ÷ 282 = $996.18

Therefore, the dashboard should display:

KPI

Correct Value

Total Tuition

$280,922.69

Average Tuition

$996.18

📊 Dashboard Charts

The dashboard contains several important charts.

1. Total Gender

A column chart showing the number of students by gender.

It includes:

Female

Male

non_gender

The chart helps compare the gender distribution.

2. Tuition by Program

A horizontal bar chart showing total tuition for each academic program.

The chart makes it easy to identify programs generating the highest tuition.

Computer Science and Data Science have the highest tuition totals.

3. Total Enrollment Status

A horizontal bar chart showing student counts by enrollment status:

Active

Deferred

Graduated

Withdrawn

non_status

This chart provides a quick overview of the current student status distribution.

4. Total Study Mode

A horizontal bar chart showing students by study mode:

Full-Time

Part-Time

Online

non_stady_mode

The chart clearly shows that Full-Time is the largest category.

5. Enrollment Date

A line chart is used to visualize enrollment counts over time.

The chart can be improved by correcting the #VALUE! issue and grouping dates by Month/Year.

🎛️ Interactive Slicers

The dashboard includes interactive slicers that allow users to filter the dashboard.

The slicers include:

Gender

Study Mode

Program

Enrollment Status

Enrollment Date

When a user selects a value from a slicer, the connected Pivot Tables and Pivot Charts update accordingly.

This makes the dashboard interactive and useful for exploring different student groups.

🔍 Key Findings

The analysis produced the following findings:

The dataset contains 300 student records.

Active students = 175, making Active the largest enrollment-status group.

Graduated students = 64.

Deferred students = 27.

Withdrawn students = 16.

Full-Time students = 162, making Full-Time the largest study mode.

Online students = 60.

Part-Time students = 59.

Computer Science has the highest total tuition at $68,526.92.

Data Science has the second-highest total tuition at $65,662.73.

Total Tuition is $280,922.69.

Average Tuition is approximately $996.18 based on 282 records containing Tuition_Fee.

The dataset contains missing values, invalid values, duplicate Student IDs, and inconsistent categories.

The Enrollment Date analysis contains a #VALUE! issue that should be corrected before final reporting.

🛠️ Excel Skills Demonstrated

This project demonstrates practical Excel data-analysis skills, including:

Data Cleaning

Handling Missing Values

Removing Duplicates

Data Standardization

Data Validation

Data Formatting

Pivot Tables

Pivot Charts

Slicers

KPI Cards

SUM

COUNT

AVERAGE

Filtering

Sorting

Date Grouping

Dashboard Design

Data Quality Analysis

📁 Suggested Workbook Structure

The Excel workbook can be organized as follows:

Student_Enrollment_Project.xlsx
│
├── Raw_Data
├── Data_Clean
├── Pivot_Tables
├── Pivot_Charts
├── Analysis
└── Dashboard

Raw_Data

Contains the original dataset before cleaning.

Data_Clean

Contains the cleaned and standardized dataset.

Pivot_Tables

Contains the Pivot Tables used for analysis.

Pivot_Charts

Contains charts created from Pivot Tables.

Analysis

Contains data-quality checks, duplicate checks, missing-value analysis, and error checks.

Dashboard

Contains the final interactive dashboard with KPIs, charts, and slicers.

🚀 Recommended Improvements

To make the project more professional and reliable:

Correct the Total Tuition KPI to $280,922.69.

Keep Average Tuition at $996.18.

Fix the #VALUE! issue in Enrollment Date.

Standardize BA to Business Administration.

Standardize CS to Computer Science.

Review NULL, Unknown, and blank values.

Review non_stady_mode.

Review non_status.

Check duplicate Student IDs.

Investigate missing Student IDs.

Create Year and Month fields for better date analysis.

Add percentage KPIs such as:

Active Rate

Graduation Rate

Withdrawal Rate

Ensure all Pivot Tables and Pivot Charts are connected to the appropriate Slicers.

Refresh all Pivot Tables after data cleaning.

🏁 Conclusion

This project is a Student Enrollment Management & Analytics Dashboard built in Microsoft Excel.

It demonstrates how raw student data can be cleaned, analyzed, and transformed into meaningful business and academic insights using Pivot Tables, Pivot Charts, KPIs, and interactive Slicers.

The project highlights important enrollment metrics such as student count, enrollment status, study mode, gender, program distribution, tuition revenue, and enrollment trends.

The analysis also demonstrates the importance of data cleaning and data quality before building a final dashboard. Correcting missing values, duplicate records, inconsistent categories, and invalid dates will make the final analysis more accurate and reliable.

👨‍💻 Project Information

Project Type: Microsoft Excel Data Analytics Project

Project Topic: Student Enrollment Management & Analytics

Main Tools: Microsoft Excel, Pivot Tables, Pivot Charts, Slicers, KPIs

Project Status: Dashboard Completed — Data Quality Improvements Recommended
