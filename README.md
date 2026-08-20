# Employee Database SQL Analysis Using DML

## Project Overview

This project demonstrates the practical use of **MySQL and SQL DML concepts** to manage and analyze employee data stored in a relational database.

The project involves creating an Employee Database, inserting structured data, performing data manipulation, and executing SQL queries to retrieve, filter, sort, aggregate, group, and join information across multiple tables.

The assignment provides hands-on practice with SQL concepts commonly used in **Data Analysis, Reporting, Business Intelligence, and Database Management**.

---

## Objectives

* Create an Employee Database using MySQL.
* Insert structured employee, department, and location data.
* Retrieve unique values using `distinct`.
* Use column aliases with `as`.
* Filter records using `where` and operators.
* Identify and update missing data.
* Sort records using `order by`.
* Limit query results using `limit`.
* Perform calculations using aggregate functions.
* Group records using `group by`.
* Filter grouped results using `having`.
* Retrieve related information using SQL joins.
* Practice `inner join`, `left join`, and `right join`.

---

## Tools Used

* **MySQL**
* **MySQL Workbench**
* **GitHub**

---

## Database Structure

The database contains three tables:

### 1. Departments

| Column          | Description                           |
| --------------- | ------------------------------------- |
| department_id   | Unique identifier for each department |
| department_name | Name of the department                |

**Total Records:** 13

### 2. Location

| Column      | Description                         |
| ----------- | ----------------------------------- |
| location_id | Unique identifier for each location |
| location    | Employee work location              |

**Total Records:** 4

### 3. Employees

| Column        | Description                |
| ------------- | -------------------------- |
| employee_id   | Unique employee identifier |
| employee_name | Name of the employee       |
| gender        | Employee gender            |
| age           | Employee age               |
| hire_date     | Employee joining date      |
| designation   | Employee job designation   |
| department_id | Department reference       |
| location_id   | Location reference         |
| salary        | Employee salary            |

**Total Records:** 30

---

## Database Relationship

The database follows a relational structure where the `employees` table connects with the `departments` and `location` tables using foreign keys.

```text
departments
     |
     | department_id
     |
employees
     |
     | location_id
     |
location
```

---

# SQL Tasks Performed

## 1. Distinct Values

Retrieved unique salary values from the `employees` table using the `distinct` keyword.

**SQL Concept:** `distinct`

---

## 2. Alias (`as`)

Provided meaningful aliases for the `age` and `salary` columns:

* `Employee_Age`
* `Employee_Salary`

**SQL Concept:** `as`

---

## 3. Where Clause & Operators

Retrieved employees who:

* Have a salary greater than ₹50,000
* Were hired before January 1, 2016

The task also identified an employee with a missing designation and updated the missing value to `Data Scientist`.

**SQL Concepts:**

* `where`
* `and`
* `is null`
* `update`

---

## 4. Order By

Sorted employees based on:

* Department ID in ascending order
* Salary in descending order

**SQL Concept:** `order by`

---

## 5. Limit

Retrieved the first five employees hired during the year 2018.

**SQL Concept:** `limit`

---

## 6. Aggregate Functions

Performed calculations using aggregate functions.

### Sum of Finance Salaries

Calculated the total salary of employees working in the Finance department.

**Function:** `sum()`

### Minimum Employee Age

Identified the minimum age among all employees.

**Function:** `min()`

---

## 7. Group By

Performed grouped analysis of employee data.

### Maximum Salary by Location

Calculated the maximum salary for each location.

**Functions:** `max()`, `group by`

### Average Salary for Analyst Designations

Calculated the average salary for each designation containing the word `Analyst`.

**Functions:** `avg()`, `group by`, `like`

---

## 8. Having

Used `having` to filter grouped results.

### Departments with Less Than 3 Employees

Identified departments having fewer than three employees.

### Female Employees with Average Age Below 30

Identified locations where female employees have an average age below 30.

**SQL Concepts:**

* `group by`
* `having`
* `count()`
* `avg()`

---

# SQL Joins

## 9. Inner Join

Retrieved:

* Employee names
* Employee designations
* Department names

for employees assigned to a department.

**SQL Concept:** `inner join`

---

## 10. Left Join

Listed all departments along with the total number of employees in each department.

The `left join` ensures that departments with no employees are also included.

**SQL Concept:** `left join`

---

## 11. Right Join

Displayed all locations along with the names of employees assigned to each location.

The `right join` ensures that all locations are displayed, even if no employees are assigned to a particular location.

**SQL Concept:** `right join`

---

# Data Manipulation

A missing designation was identified in the employee data and updated using an `update` statement.

The missing designation was filled with:

```text
Data Scientist
```

This demonstrates a basic SQL data-cleaning and data-manipulation operation.

---

# SQL Concepts Covered

The following SQL concepts were practiced in this project:

```text
select
distinct
as
where
and
is null
update
order by
limit
sum()
min()
avg()
max()
count()
group by
having
like
inner join
left join
right join
```

---

# Key Learning Outcomes

Through this project, I gained practical experience in:

* Writing SQL queries for data retrieval
* Filtering and sorting relational data
* Performing data manipulation
* Handling missing values
* Using aggregate functions
* Performing grouped analysis
* Applying conditional filtering with `having`
* Understanding primary and foreign key relationships
* Joining multiple tables
* Analyzing employee and organizational data

---

# Screenshots

All assignment screenshots are stored separately in the `Screenshots` folder.

The folder contains screenshots demonstrating the execution and results of each SQL task.

Screenshots


Distinct_Salaries
<img width="881" height="182" alt="image" src="https://github.com/user-attachments/assets/5fa4e93f-994b-4106-8afa-9e99414feed2" />






Alias_AS_Age_Salary
<img width="771" height="127" alt="image" src="https://github.com/user-attachments/assets/99bd370c-0b5e-4046-8d89-3ce5fc24a98e" />









Where_Salary_And_Hire_Date
<img width="785" height="135" alt="image" src="https://github.com/user-attachments/assets/fa291c7b-a185-40b3-a563-b938cf86be93" />






Find_Missing_Designation




<img width="849" height="320" alt="image" src="https://github.com/user-attachments/assets/b5f6a6a1-1c97-4931-9c24-f2397d67a0df" />





Update_Missing_Designation




<img width="836" height="195" alt="image" src="https://github.com/user-attachments/assets/0702f1ef-1e3e-4187-816c-31cb556dc3c0" />








├── Order_By_Department_Salary




<img width="336" height="125" alt="image" src="https://github.com/user-attachments/assets/130c8d8c-8576-4c29-9ce8-f01ffd93e74c" />






Limit_First_5_Employees_2018




<img width="337" height="103" alt="image" src="https://github.com/user-attachments/assets/7df2a1b9-3f05-4a42-8240-5c9d01a0c8b4" />






Sum_Salary_Finance_Department



<img width="313" height="142" alt="image" src="https://github.com/user-attachments/assets/30309af7-de87-4edd-9f35-6c3743bfffe8" />








Minimum_Age_Employees




<img width="358" height="201" alt="image" src="https://github.com/user-attachments/assets/aa754a2e-6954-4a05-92d2-9a5c745ce723" />








Maximum_Salary_Each_Location



<img width="423" height="213" alt="image" src="https://github.com/user-attachments/assets/05f476d0-82b1-46b5-b008-91b55d02bb6e" />






Average_Salary_Analyst_Designations




<img width="239" height="117" alt="image" src="https://github.com/user-attachments/assets/d55492e5-76b3-4991-87bb-8bbb5615e1de" />








Departments_Less_Than_3_Employees



<img width="475" height="370" alt="image" src="https://github.com/user-attachments/assets/5f8c8d2c-066a-4143-926e-73135e06533e" />





Locations_Female_Average_Age_Below_30




<img width="470" height="324" alt="image" src="https://github.com/user-attachments/assets/50741268-56bb-4035-b318-331a642901c5" />








Inner_Join_Employees_Departments



<img width="226" height="369" alt="image" src="https://github.com/user-attachments/assets/69592b85-18c3-47a0-873d-d96cbb240e78" />








Left_Join_Departments_Employee_Count



![Uploading image.png…]()




Right_Join_Locations_Employees


![Uploading image.png…]()









# Repository Structure

```text
employee-database-sql-analysis-dml/
│
├── README.md
│
├── SQL/
│   └── Employee_Database.sql
│
└── Screenshots/
    ├── Distinct_Salaries.png
    ├── Alias_AS_Age_Salary.png
    ├── Where_Salary_And_Hire_Date.png
    ├── Find_Missing_Designation.png
    ├── Update_Missing_Designation.png
    ├── Order_By_Department_Salary.png
    ├── Limit_First_5_Employees_2018.png
    ├── Sum_Salary_Finance_Department.png
    ├── Minimum_Age_Employees.png
    ├── Maximum_Salary_Each_Location.png
    ├── Average_Salary_Analyst_Designations.png
    ├── Departments_Less_Than_3_Employees.png
    ├── Locations_Female_Average_Age_Below_30.png
    ├── Inner_Join_Employees_Departments.png
    ├── Left_Join_Departments_Employee_Count.png
    └── Right_Join_Locations_Employees.png
```

---

# Conclusion

This Employee Database SQL project demonstrates the practical application of **SQL DML, data retrieval, aggregation, grouping, filtering, data manipulation, and table joins** using MySQL.

The project strengthened my understanding of relational databases and SQL techniques used for real-world data analysis and reporting.

It serves as a practical demonstration of SQL skills relevant to an **Aspiring Data Analyst**.

---

## Author

**Kumar**

**Data Analyst**

**Skills Demonstrated:**
`SQL` · `MySQL` · `DML` · `Data Analysis` · `Data Manipulation` · `Data Cleaning` · `Aggregate Functions` · `SQL Joins`
