# Tlias Project Demo

## Project Overview
This project is a **Class Management System** that includes Employee Management, Class Management, Student Management, and Violation Records Management.  
- **Frontend:** Vue3 + Element Plus  
- **Backend:** Spring Boot  
- **Database:** MySQL  

The project is suitable for resume demonstration, allowing interviewers to quickly review the project structure, setup, and sample data.

---

## Repository Structure
tlias-project-demo/
├─ frontend/ # Frontend build files
│ └─ dist/
│ ├─ index.html
│ ├─ favicon.ico
│ └─ assets/
├─ backend/ # Backend build file
│ └─ tlias-web-management-1.0-SNAPSHOT.jar
├─ database/ # Database SQL file
│ └─ student_db_schema.sql
└─ README.md # Project documentation

yaml
Copy
Edit

---

## Database
- SQL file path: `database/student_db_schema.sql`  
- Includes tables: Departments, Employees, Classes, Students, Student Records, and related Logs  
- Contains a small set of **English sample data** for demo purposes:  
  - Student names: Tom, Anna  
  - Employee names: John Smith, Emily Jones  
  - Phone numbers: start with `01` followed by 8 digits  
- Foreign key relationships are complete. Import the SQL file to run the backend service.

---

## Frontend Setup
- The frontend is pre-built; open `frontend/dist/index.html` directly to view the application.  
- For development purposes, set up Node.js + Vue3 environment and refer to Vue3 + Element Plus documentation.

---

## Backend Setup
- Run the backend JAR file with Java:

```bash
java -jar backend/tlias-web-management-1.0-SNAPSHOT.jar
Make sure to import the student_db_schema.sql file into MySQL.

Update database connection information in application.properties (username, password, port, etc.).

Usage Instructions
Import the database SQL file

Start the backend JAR

Open frontend/dist/index.html in a browser to access the system

Technology Stack
Frontend: Vue3 + Element Plus

Backend: Spring Boot 2.x

Database: MySQL 8.x

Build Tool: Maven

Demo Data
Departments: Development, HR

Employees: John Smith, Emily Jones

Classes: Java Class 01, Frontend Class 01

Students: Tom, Anna

Student Violations: Late, Fight (English descriptions)

Notes
This project is intended as a resume-friendly demo, showing the integration of frontend, backend, and database.

Log tables (emp_log, student_log, operate_log) are empty but can be extended as needed.