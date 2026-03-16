# Library-Management-System
📚 Library Management System (MySQL)
📌 Project Description

The Library Management System is a database project developed using MySQL to manage library operations.
It stores and manages information about books, employees, customers, and book transactions such as issuing and returning books.

This system helps libraries efficiently track:

Book availability

Customer registrations

Book issue and return records

Employee and branch information

🗄 Database Name
library
📊 Tables Used in the Project
1️⃣ Branch

Stores information about library branches.

Column	Description
Branch_no	Primary key of branch
Manager_Id	Manager of the branch
Branch_address	Address of the branch
Contact_no	Branch contact number
2️⃣ Employee

Stores employee details.

Column	Description
Emp_Id	Primary key
Emp_name	Employee name
Position	Job position
Salary	Employee salary
Branch_no	Foreign key referencing Branch
3️⃣ Books

Stores information about books available in the library.

Column	Description
ISBN	Primary key
Book_title	Title of the book
Category	Book category
Rental_Price	Rental price of the book
Status	Availability (Yes/No)
Author	Book author
Publisher	Book publisher
4️⃣ Customer

Stores customer information.

Column	Description
Customer_Id	Primary key
Customer_name	Name of customer
Customer_address	Address
Reg_date	Registration date
5️⃣ IssueStatus

Stores book issue records.

Column	Description
Issue_Id	Primary key
Issued_cust	Foreign key referencing Customer
Issued_book_name	Name of issued book
Issue_date	Date of issue
Isbn_book	Foreign key referencing Books
6️⃣ ReturnStatus

Stores book return records.

Column	Description
Return_Id	Primary key
Return_cust	Customer returning book
Return_book_name	Returned book name
Return_date	Return date
Isbn_book2	Foreign key referencing Books
🔍 SQL Queries Implemented

The project includes queries to perform the following operations:

Retrieve available books with category and rental price

List employees with salary in descending order

Show customers who issued books

Count books in each category

Find employees with salary above ₹50,000

Customers registered before 2022 who have not issued books

Number of employees in each branch

Customers who issued books in June 2023

Search books containing the word History

Branches having more than 5 employees

Employees managing branches with branch address

Customers who issued books with rental price greater than ₹25

🛠 Technologies Used

MySQL

SQL Queries

Relational Database Concepts

▶️ How to Run the Project

Install MySQL Server or MySQL Workbench

Create the database:

CREATE DATABASE library;
USE library;

Run the SQL scripts to create tables

Insert sample data

Execute the queries to test the system

🎯 Project Purpose

This project demonstrates the use of:

SQL table creation

Primary and foreign keys

Data retrieval using queries

JOIN operations

GROUP BY and HAVING clauses

It is suitable for Database Management System (DBMS) learning and academic projects.
