# Student Enrollment Management System

## Description

A SQL-based database management project designed to manage students, courses, and enrollments efficiently. The system stores student information, course details, and enrollment records while maintaining relationships between tables using foreign keys.

## Features

* Manage student records
* Manage course information
* Enroll students in courses
* Maintain relationships between students and courses
* Track enrollment dates automatically
* Retrieve enrollment information using SQL JOIN operations

## Technologies Used

* SQL
* MySQL

## Database Concepts Used

### Database Creation

* Created a dedicated database using SQL

### Table Design

* Students Table
* Courses Table
* Enrollment Table

### Primary Keys

* Unique identification for students, courses, and enrollments

### Foreign Keys

* Maintains relationships between tables
* Ensures data integrity

### Constraints

* PRIMARY KEY
* FOREIGN KEY
* UNIQUE
* NOT NULL
* AUTO_INCREMENT

### Data Manipulation Language (DML)

* INSERT statements for adding records

### Query Operations

* SELECT statements
* INNER JOIN operations
* Filtering records using WHERE clause

## Database Schema

### Students Table

| Column       | Data Type    |
| ------------ | ------------ |
| student_id   | INT          |
| student_name | VARCHAR(100) |
| email        | VARCHAR(100) |
| dob          | DATE         |

### Courses Table

| Column      | Data Type    |
| ----------- | ------------ |
| course_id   | INT          |
| course_name | VARCHAR(100) |
| description | TEXT         |
| credits     | INT          |

### Enrollment Table

| Column          | Data Type |
| --------------- | --------- |
| enrollment_id   | INT       |
| student_id      | INT       |
| course_id       | INT       |
| enrollment_date | DATETIME  |

## Sample Operations

### Add Students

* Store student details
* Maintain unique email records

### Add Courses

* Store course information
* Track course credits

### Student Enrollment

* Assign students to courses
* Record enrollment timestamps

### Enrollment Report

Retrieve enrolled courses for a specific student using JOIN queries.

## How to Run

1. Install MySQL Server.
2. Open MySQL Workbench or any SQL client.
3. Execute the SQL script.
4. Database, tables, and sample data will be created automatically.
5. Run the provided SELECT queries to view enrollment information.

## Project Structure

```text
StudentEnrollmentManagementSystem/
│
└── student_enrollment.sql
```

## Learning Outcomes

* Relational Database Design
* Database Normalization
* Table Relationships
* SQL Query Writing
* Data Integrity Management
* Join Operations
* Constraint Management

## Future Enhancements

* Student attendance tracking
* Faculty management module
* Course registration portal
* Performance and grade management
* Integration with a Java Spring Boot application

## Author

Sai Sreehas
