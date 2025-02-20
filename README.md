# Employee Management System README

## Overview

The **Employee Management System** is designed to manage and track key employee-related data, such as **departments**, **salaries**, and **performance reviews**. The system is implemented in a relational database, and the project provides queries to extract useful insights from the data.

This README will explain the key features of the database, including table structures, sample data, and common queries that can be run to analyze and manipulate the data.

---

## Features

### 1. **Departments Table**
The `Departments` table stores the names of different departments within the company (e.g., HR, IT, Sales, etc.). Each department is identified by a unique `department_id`.

### 2. **Employees Table**
The `Employees` table contains basic information about employees, including:
- `employee_id`: A unique identifier for each employee.
- `first_name` & `last_name`: Personal details of the employee.
- `department_id`: A foreign key that links each employee to a specific department.
- `hire_date`: The date when the employee joined the company.

### 3. **Salaries Table**
The `Salaries` table records salary details for each employee. It includes:
- `salary_id`: A unique identifier for each salary record.
- `employee_id`: A foreign key that links the salary record to the relevant employee.
- `salary`: The amount the employee earns.
- `salary_date`: The date the salary was recorded.

### 4. **Performance Reviews Table**
The `Performance_Reviews` table stores performance evaluations for each employee. This includes:
- `review_id`: A unique identifier for each review.
- `employee_id`: A foreign key linking the review to an employee.
- `review_date`: The date the review was conducted.
- `performance_rating`: A numeric score (between 1 and 5) that reflects the employee’s performance.
- `comments`: Optional feedback provided during the review.

---

## Data Management

### Inserting Data
Sample data is inserted into the tables to demonstrate typical entries:
- **Departments**: Adds basic departments like HR, IT, Sales, and Business.
- **Employees**: Adds employees with their first and last names, assigned departments, and hire dates.
- **Salaries**: Adds salary information for the employees, including the salary amount and date.
- **Performance Reviews**: Adds performance ratings and comments for each employee, linked to their reviews.

### Queries
The system supports several useful SQL queries to extract insights and manage the employee data:

1. **Select All Employees with Salary Above a Specific Threshold**: 
   - This query retrieves a list of employees whose salary exceeds a specific value (e.g., 40,000).

2. **Find Employees with Poor Performance**: 
   - This query identifies employees who have received a performance rating below a threshold (e.g., rating below 3).

3. **Retrieve Employees with Reviews After a Certain Date**: 
   - This query returns employees who had performance reviews after a specific date (e.g., after 2020).

4. **Retrieve Employees with Reviews Before a Certain Date**: 
   - This query identifies employees who had performance reviews before a specific date (e.g., before 2021).

---

## Use Cases

This system can be used for:
- **Employee performance tracking**: Checking who performed poorly or well in reviews.
- **Salary management**: Identifying high-earning employees or analyzing salary distributions.
- **Department-wise analysis**: Sorting employees by department and viewing relevant details.

---

## Conclusion

The **Employee Management System** provides a structured way to manage employee data, track performance, and manage payroll, all while allowing for easy querying and reporting. You can extend this database with additional tables and queries as per your organization's needs.
