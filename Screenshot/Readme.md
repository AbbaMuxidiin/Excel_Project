


Student Enrollment Data Analysis Using Excel
Project Overview
This project analyzes a Student Enrollment dataset using Microsoft Excel. The workbook demonstrates a complete workflow from raw data quality checking and cleaning to PivotTables, PivotCharts, KPIs, and dashboard planning.

Dataset
Raw data sheet: Enrollment_Row

Cleaned data sheet: Data_clean

Rows: 300

Main analysis columns: Student_ID, Gender, Program, Enrollment_Date, Study_Mode, Tuition_Fee, Enrollment_Status

Additional derived columns in Data_clean: Year, Monthly, Clean_Enrollment_Date

Data Quality
The raw dataset contains intentionally introduced missing/invalid values for cleaning practice.

Total blank cells across the 7 main columns: 115

Duplicate full rows: 6

Repeated Student IDs: 22

Cleaning should include:

Detect and review missing values.

Standardize text categories such as Gender, Program, Study Mode, and Enrollment Status.

Validate dates and convert them to a consistent date format.

Review invalid tuition values and convert the field to numeric.

Check Student_ID uniqueness and investigate duplicates.

Keep the cleaned dataset as the reporting source.

Key KPIs
Total Students: 300

Active Students: 175

Graduated Students: 64

Withdrawn Students: 16

Total Tuition: 280,922.69

Average Tuition: 936.41

Main Analysis
Recommended business questions:

Which program has the highest enrollment?

What is the gender distribution?

Which study mode is most popular?

What is the total and average tuition?

What is the enrollment-status distribution?

How does enrollment change over time?

Which program produces the highest tuition total?

How does tuition differ by study mode?

PivotTables / PivotCharts
The workbook includes analysis sheets for:

Enrollment by Gender

Enrollment by Program

Enrollment Status

Tuition by Program

Study Mode

Enrollment by Date/Month

Tuition by Study Mode

Suggested PivotCharts:

Bar/Column chart for Program enrollment

Doughnut chart for Enrollment Status

Column/Bar chart for Gender

Doughnut/Pie chart for Study Mode

Line chart for monthly enrollment trend

Column chart for Tuition by Program

Dashboard
The Analysis sheet contains the recommended dashboard structure.

KPI Cards
Total Students

Active Students

Graduated Students

Total Tuition

Filters / Slicers
Year

Program

Gender

Study Mode

Enrollment Status

Recommended Layout
Top: KPI cards
Middle: Program, Status, Gender/Study Mode charts
Bottom: Enrollment trend and Tuition by Program
Side/Top: Slicers

Workbook Structure
Project_Index — project/student index

Enrollment_Row — raw enrollment dataset

Data_clean — cleaned/reporting dataset

Analysis — analysis summary, KPIs, data quality, and dashboard plan

Dashboard / DASHBOARD2 — dashboard-related sheets

Pivot* sheets — PivotTable analysis outputs

Analaysi_data — existing data-quality analysis sheet

Tools Used
Microsoft Excel

PivotTables

PivotCharts

Excel formulas

Data cleaning

Dashboard design

Project Goal
The goal is to transform raw student enrollment records into a clean, understandable, and decision-ready Excel report with measurable KPIs and interactive visual analysis.
