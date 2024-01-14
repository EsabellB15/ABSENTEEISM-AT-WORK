# ABSENTEEISM-AT-WORK

![Intro_image](https://github.com/EsabellB15/ABSENTEEISM-AT-WORK/assets/123163220/4d51fefc-cf7f-4ea0-bf05-54979e5bdcb7)

## Introduction
This is a Power BI project on Absenteeism at work analysis.  I worked on this project to practice my skills in data cleaning, analysis, and visualization.

## Problem Statement
1.	Determine if there are overall trends in absenteeism over a specified period (Monthly).
2.	Determine if there are any seasonal patterns in absenteeism.
3.	Investigate if absenteeism varies by day of the week.
4.	Analyse the primary reasons for absenteeism.
5.	Investigate the relationship between workload and absenteeism.
6.	Investigate the relationship between transportation expenses and workload.

## Data Sourcing
I downloaded the CSV file from absent data and extracted it into Power BI for cleaning, analysis, and visualization.
-	Data has 3 sheets/tables comprising employee records, compensation, and tracked absences.
- The employee records table has 21 Columns and 740 rows.
-	The compensation table has 2 Columns and 740 rows.
-	The reasons table has 2 Columns and 29 rows.

## Data Cleaning
-	The data was clean, I just double-checked to ensure there was no missing data, duplicate data, or inconsistent data, and that data types were correct.
-	Calculate a new measure of the average time of absence in hours.
-	Calculate a new measure of the total number of employees.
-	Calculate a new measure of the total hours of absence at work by employees.
-	Calculated a new column of the BMI of the employee using DAX.
-	Calculated a new column of the season to convert seasons from numbers to text and used the month of absence in the Dax calculation.

![Data_cleaning](https://github.com/EsabellB15/ABSENTEEISM-AT-WORK/assets/123163220/55f0aa01-f8b7-4dc6-b212-f2873cec46a1)

## Data Modelling
-	Power BI automatically connected two related tables, the absenteeism_at_work table, and the compensation table. I had to change the cardinality of this from one to one(1:1) to many to one(*:1) and the cross-filter direction from both to single.
-	I then connected the absenteeism_at_work table with the Reasons table via the common columns:  ‘Reason for absence’ and ‘Number’.
-	This connection resulted in a star schema model.

![Data_model](https://github.com/EsabellB15/ABSENTEEISM-AT-WORK/assets/123163220/e3392cb0-8bf1-4345-9cfb-ac49e0044d6c)

## Data Analysis 

![Data_Analysis](https://github.com/EsabellB15/ABSENTEEISM-AT-WORK/assets/123163220/ef399394-df03-4bdb-b7c8-88b3ba0c5b6f)

You can interact with this report [here]( https://app.powerbi.com/groups/13bfa296-3bf8-4464-86eb-f48267f0fff7/reports/3554c028-f146-4757-9280-5d1a5b260238/ReportSection?redirectedFromSignup=1&experience=power-bi)

## Conclusions
-	Observation:  More employees take absentee leave in warmer seasons, with Spring having the highest absenteeism. 
-	Observation: July has the highest average absenteeism hours, followed by the spring months. 
-	Observation: Employees are more likely to be absent in the early days of the week. 
-	Observation: No correlation between workload and transportation expenses.
-	Observation: Medical conditions are the primary reason for absenteeism. 
-	Observation: More employees are overweight or obese, potentially contributing to medical condition-related absenteeism.
-	Observation: Many employees have lower education levels, possibly impacting health awareness

## Recommendations
-	Investigate specific factors causing higher absenteeism in warmer seasons, especially during Spring.
-	Implement strategies to manage absenteeism during July and warmer months.
-	Conduct in-depth analysis to understand and address the reasons behind higher absenteeism early in the week.
-	Introduce programs to promote employee health and combat absenteeism, considering the observed high BMI rates.
-	Develop initiatives to enhance health awareness, especially among employees with lower education levels, to reduce absenteeism.







