# INTRODUCTION

This is a Microsoft Excel Project focused on understanding employee attrition patterns. This project was carried out in an attempt to analyze and monitor employee attrition trends within an organization. 

Employee attrition analytics focused on identifying why employees voluntarily leave, what might prevented them from leaving, and how we can use data to predict attrition risk. In addition, this type of employee predictive analytics can be used to help organizations understand and design the interventions that will be most effective in reducing unwanted attrition.

## DATA OVERVIEW
The HR attrition dataset comprises 1,470 rows and 35 columns, each shedding light on various aspects of the organizational environment. Key features such as employee number, age, and gender provide essential demographic insights into the workforce. The "attrition" column, categorized into "yes" and "no," serves as the focal point for analyzing employee turnover. Additional variables, including department, marital status, job involvement, satisfaction levels, monthly income, and tenure metrics like years in the current role and years since the last promotion, offer a comprehensive view of organizational dynamics. This dataset forms the foundation for an in-depth exploration of the factors influencing attrition, enabling a nuanced analysis of how personal and professional elements impact the employee experience.

Additionally, the dataset includes a column for attrition which indicates whether an employee has the left the company or is still employed. 

## DATA CLEANING PROCESS

The first step in the project involved data cleaning to ensure accuracy in the dataset analysis. This involves sorting, removing duplicates in the entry of the data to avoid potential biases, checking for missing data and correct data type in each column. 
I utilized the following steps for the data cleaning process;

**Data Importation**: The first thing I did was to import my dataset by clicking on the data ribbon. The dataset was in CSV format, so I convert it to …. As shown below
		
![](Data.png)

**Data Cleaning**: 

_**Removing duplicates**_: I checked for duplicates by clicking on the remove duplicates on the Data Ribbon. 7 duplicates were discovered as shown in the image below;
					
![](Duplicate.png)

_**Column checking**_: I filtered each column to check for missing and outliers in the data. I also checked for accuracy in the data type for each column. The dataset was devoid of missing data and outliers. 
					
![](ColumnChecking.png)

_**Replacing Values**_: I replaced the column JobRole contains number 1-4. From the dataset source, they represent the following:

**Job Satisfaction**

1 = very dissatisfied

2 = dissatisfied

3 = satisfied

4 = very satisfied

**Environment Satisfaction**

1 = Low

2 = Medium

3 = High

4 = Very High

**Education Level**

1 = High School

2 = Associate

3 = Bachelor's degree

4 = Master's degree

5 = Doctorate degree

## DATA ANALYSIS

### BUSINESS QUESTIONS

To further answer the pending questions on employee attrition, the following answers were provided.

**Total Employees**: The COUNT function was used, that is =COUNT(K2:K1474). And the value is 1473

**Active Employees**: The COUNTIF function was used, that is =COUNTIF(D2:D1474, "=No"). And the value is 1236

**Attrition Employees**: The COUNTIF function was used, that is =COUNTIF(D2:D1474, "=Yes"). And the value is 237

**Attrition Rate**: The DIVISION function was used, that is = Attrition Employess/Total Employees * 100. And the value is 16%

**Attrition Female Employees**: The COUNTIFS function was used, that is =COUNTIFS(D2:D1474, "=Yes", N2:N1474, "=Female"). And the value is 87

**Attrition Male Employees**: The COUNTIFS function was used, that is =COUNTIFS(D2:D1474, "=Yes", N2:N1474, "=Male"). And the value is 150

**Average Age**: The AVERAGE function was used, that is =AVERAGE(B2:B1474).And the value is 37

**Average Salary**: The AVERAGE function was used, that is =AVERAGE(U2:U1474).And the value $6500.00



## PIVOT TABLE

_ATTRITION BT EDUCATION_

A doughnut chart was utilized to effectively compare the proportions of attrition of the employees at the company with education.
![](AttritionbyEdu.png)

_ATTRITION BY AGEGROUP BY GENDER_

A stacked column chart was utilized to effectively compare the proportions of attrition of the employees at the company with gender and age group.

![](AttritionbyAgebyGender.png)

_ATTRITION BY YEARS AT COMPANY_

An area chart was utilized to effectively depict the relationship between attrition of the employees at the company with years at company.
![](AtrritionbyYears.png)

_ATTRITION BY MARITAL STATUS_

A pie chart was utilized to effectively compare the proportions of attrition of the employees at the company with marital status.
![](AttritionbyMaritalstatus.png)

_ATTRITION BY JOB SATISFACTION_

_ATTRITION BY EDUCATION LEVEL_

_ATTRITION BY JOB LEVEL_

ATTRITION BY SALARY

A bar chart was utilized to effectively compare the proportions of attrition of the employees at the company with salary earned.
![](AttritionbySalary.png)

ATTRITION BY DEPARTMENT

A pie chart was utilized to effectively compare the proportions of attrition of the employees at the company with department.
![](AttritionbyDept.png)


## INSIGHTS AND RECOMMENDATION
After the analysis
1. The total employee count is 1473 with attrition rate of 16%
2. The attrition rate among the male employees was the highest at 63%
3. 
4. Age group 26-37 had the highest attrition count of 116 employees
5. Employees that are single had the highest atrrition rate of 51%, followed by married 35% and the divorced 14%
6. Employees from the Research & Development had attrition rate of 56%, HR had 39%, and Sales had 5%
7. Employees with up to 5K monthly income had the highest attrition count of 163
8. Entry level employees faced the highest attrition, while the senior employees had the lowest turnover

## RECOMMENDATIONS

