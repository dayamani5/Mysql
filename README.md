Python MySQL Database Management System (DBMS)

This project demonstrates how to connect Python with MySQL and perform basic database operations such as creating databases, creating tables, inserting data, displaying records, updating data, and deleting records.

It is a beginner-friendly example of using Python as a backend for DBMS operations.

Features

Connect Python to MySQL server

Create a database automatically

Create tables with primary and foreign keys

Insert multiple records safely

Display data using SELECT and JOIN queries

Update existing records

Delete records while maintaining referential integrity

Reset tables and auto-increment values

Technologies Used

Python

MySQL

mysql-connector-python

Database Details

Database Name: SchoolDB

Tables
Students
Column	Type
id	INT (Primary Key, Auto Increment)
name	VARCHAR(100)
age	INT
grade	VARCHAR(10)
Classes
Column	Type
class_id	INT (Primary Key, Auto Increment)
student_id	INT (Foreign Key)
subject	VARCHAR(50)
score	INT
Project Structure
python-mysql-dbms/
│
├── dbms.py
└── README.md

Installation and Setup

Install MySQL

Make sure MySQL Server is installed and running

Install Python MySQL Connector

pip install mysql-connector-python


Update MySQL Credentials
Edit these values in the code:

create_connection("localhost", "root", "your_password")


Run the program

python dbms.py

Program Flow

Connects to MySQL server

Creates SchoolDB database if it does not exist

Connects to SchoolDB

Creates Students and Classes tables

Clears old data and resets auto-increment

Inserts sample student and class data

Displays student records

Displays joined student-subject-score data

Updates student grade

Deletes a student and related records safely

Sample Operations Performed

INSERT → Add new students and scores

SELECT → Fetch all records

JOIN → Display student names with subject scores

UPDATE → Modify student grade

DELETE → Remove student and dependent records

Output

Displays student table records

Displays joined student score records

Shows updated and deleted data results

Notes

Foreign key checks are temporarily disabled during table reset

Sample data is safely inserted using parameterized queries

Make sure MySQL service is running before execution

Learning Outcomes

Python–MySQL connectivity

Database creation and management

SQL queries from Python

Handling foreign key relationships

CRUD operations using Python

Author

Dayamani
B.Tech CSE (AI & ML)
Python MySQL DBMS Project
