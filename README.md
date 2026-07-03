# Student Enrollment Management System

## Description

The Student Enrollment Management System is a SQL-based database project developed to manage student records, course information, and enrollments efficiently. The project demonstrates relational database concepts such as table relationships, primary and foreign keys, constraints, and SQL queries for data retrieval.

## Features

- Manage student records
- Store course information
- Enroll students in courses
- Maintain relationships using foreign keys
- Automatically record enrollment dates
- Retrieve enrollment details using SQL JOIN queries
- Ensure data integrity through database constraints

## Technologies Used

- MySQL
- SQL

## Database Tables

### Students
- student_id (Primary Key)
- student_name
- email
- dob

### Courses
- course_id (Primary Key)
- course_name
- description
- credits

### Enrollment
- enrollment_id (Primary Key)
- student_id (Foreign Key)
- course_id (Foreign Key)
- enrollment_date

## SQL Concepts Used

- Database Creation
- Table Creation
- Primary Keys
- Foreign Keys
- AUTO_INCREMENT
- NOT NULL Constraint
- UNIQUE Constraint
- INSERT Statements
- SELECT Queries
- INNER JOIN
- WHERE Clause

## Project Structure

```text
StudentEnrollmentManagementSystem/
│── student_enrollment.sql
```

## How to Run

1. Install MySQL Server.
2. Open MySQL Workbench or any SQL client.
3. Execute the `student_enrollment.sql` file.
4. The database, tables, and sample records will be created automatically.
5. Run the provided SELECT queries to retrieve enrollment details.

## Sample Query

```sql
SELECT s.student_name, c.course_name, e.enrollment_date
FROM Students s
JOIN Enrollment e ON s.student_id = e.student_id
JOIN Courses c ON e.course_id = c.course_id
WHERE s.student_id = 1;
```

## Learning Outcomes

- Relational Database Design
- SQL Query Writing
- Table Relationships
- Data Integrity Management
- JOIN Operations
- Constraint Implementation

## Future Enhancements

- Student attendance management
- Faculty management
- Grade management
- Course registration portal
- Integration with a Java Spring Boot application

## Author

**Sai Sreehas**
