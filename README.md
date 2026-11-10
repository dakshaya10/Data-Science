College Library Management System
1. Project Overview
The College Library Management System is a database management project developed using MySQL. It is designed to manage library members, book details, and book issuing and returning records efficiently.
The system maintains information about students, faculty members, available books, and book transactions using relational database concepts.
2. Objectives
•	To maintain member details.
•	To store and manage book information.
•	To record book issuing and returning details.
•	To maintain relationships between members and books.
•	To reduce manual record-keeping.
•	To understand and implement SQL database concepts.
3. Technologies Used
•	Database: MySQL
•	Language: SQL
•	Tool: MySQL Workbench / MySQL Command Line
4. Database Name
librarydb
5. Database Tables
The project consists of three main tables:
A. Members Table
Stores information about library members.
Column Name	Data Type	Description
member_id	INT	Primary Key
member_name	VARCHAR(100)	Member Name
member_type	ENUM	Student / Faculty
joined_date	DATE	Joining Date
B. Books Table
Stores information about books available in the library.
Column Name	Data Type	Description
book_id	INT	Primary Key
title	VARCHAR(150)	Book Title
author	VARCHAR(100)	Author Name
category	VARCHAR(100)	Book Category
price	DECIMAL(10,2)	Book Price
copies_available	INT	Available Copies
C. Issues Table
Stores information about books issued to members.
Column Name	Data Type	Description
issue_id	INT	Primary Key
member_id	INT	Foreign Key
book_id	INT	Foreign Key
issue_date	DATE	Issue Date
due_date	DATE	Due Date
return_date	DATE	Return Date
6. Relationships
The database contains the following relationships:
•	One member can have multiple book issue records (1).
•	One book can appear in multiple issue records (1).
•	The member_id in the Issues table references the Members table.
•	The book_id in the Issues table references the Books table.
7. SQL Concepts Used
•	CREATE DATABASE
•	USE DATABASE
•	CREATE TABLE
•	PRIMARY KEY
•	FOREIGN KEY
•	AUTO_INCREMENT
•	NOT NULL
•	ENUM
•	DEFAULT
•	SHOW TABLES
•	DESC
8. How to Execute the Project
1.	Install MySQL on your computer.
2.	Open MySQL Workbench or MySQL Command Line.
3.	Copy the SQL source code.
4.	Execute the SQL statements.
5.	Select the librarydb database.
6.	Execute SHOW TABLES; to verify table creation.
7.	Execute DESC members;, DESC books; and DESC issues; to view the table structures.
9. Expected Output
After successful execution, the database will contain three tables:
•	members
•	books
•	issues
These tables are connected through primary key and foreign key relationships.
10. Conclusion
The College Library Management System demonstrates the practical implementation of relational database concepts using MySQL. It provides a structured way to store and manage library members, books, and issue records.
This project helps in understanding database creation, table relationships, primary keys, foreign keys, and SQL commands.
________________________________________
Project Title: College Library Management System
Database: MySQL


"# Data-Science" 
