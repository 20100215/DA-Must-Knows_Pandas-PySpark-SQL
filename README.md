# Data Analytics Must Knows

### Pandas, SQL, PySpark

![portfolio-18](https://github.com/user-attachments/assets/4a236017-1f3a-41ea-8987-69de2ee89461)

Situation: 

You are given two sets of JSON data (employees info, bonuses info) formatted as a string which holds basic employee information in a company that has several departments, and you are given a series of analytics questions to analyze. 

You are to provide your solutions to each question in every language/library - **Pandas**, **SQL**, and **PySpark**.

**View the Solution Notebook here: [Solution Link](https://github.com/20100215/DA-Must-Knows_Pandas-PySpark-SQL/blob/main/notebook.ipynb)**

### Data:


1. `employees_json` 
``` 
[
    {"EmployeeID":1, "Name":"Alice", "Department":"HR", "Salary":60000, "JoiningDate":"2019-01-15", "PerformanceScore":3},
    {"EmployeeID":2, "Name":"Bob", "Department":"IT", "Salary":70000, "JoiningDate":"2019-06-20", "PerformanceScore":4},
    {"EmployeeID":3, "Name":"Charlie", "Department":"IT", "Salary":80000, "JoiningDate":"2018-07-23", "PerformanceScore":2},
    {"EmployeeID":4, "Name":"David", "Department":"HR", "Salary":65000, "JoiningDate":"2020-02-10", "PerformanceScore":5},
    {"EmployeeID":5, "Name":"Eve", "Department":"Finance", "Salary":75000, "JoiningDate":"2021-03-15", "PerformanceScore":3}
]
```
2. `bonuses_json`
```
[
    {"EmployeeID":1, "Bonus":5000},
    {"EmployeeID":2, "Bonus":7000},
    {"EmployeeID":3, "Bonus":8000},
    {"EmployeeID":6, "Bonus":6000}
]
```

### Questions:

Q0: Import the necessary libraries and perform the necessary setup to complete the tasks for all the indicated languages and libraries.

Q1: How can you calculate the average salary for each department?

Q2: Determine the employee with the highest performance score in each department.

Q3: Add a new column that represents the number of years each employee has been with the company based on the JoiningDate.

Q4: Create a pivot table to display the total salary and average performance score for each department.

Q5: Create a new DataFrame containing only the employees from the IT department who have a performance score greater than 3.

Q6: Perform an merge of the employees data with the bonuses data based on EmployeeID and keep only the employees that exist in the employees data. Impute the missing values appropriately.

Q7: Calculate the cumulative average of the PerformanceScore column grouped by Department, ordered by joining date.

Q8: Rank the employees within each department based on their Salary.

Q9: Show the count of employees per department who have been with the company for more than 4 years. Include departments with no such employees. Order the result by descending order of count of employees meeting the criteria.

Q10 (A): Calculate the total salary dispensed by the company each year for the years 2018 until 2024.

Assume that salaries are paid at the end of the year equivalent to the amount indicated in the 'Salary' column if the employee is able to work for that full year, or a fractional amount of the salary (floored) depending on the length worked by the employee on his starting year (e.g. Joining date: 2020-12-01 -> floor(Salary * 30 / 365) -> since there are 30 days left till the end of the year).

Q10 (B): Create a pivot table of the total annual salaries dispensed in (A) by breaking down the totals by department.
