# SQL_Banking_Assignment
Description
This repository contains SQL scripts for managing and analyzing a banking dataset. The dataset models a simple banking system with tables for products, employees, customers, accounts, transactions, and customer-account relationships. The assignment demonstrates  performing data analysis with SQL.

Dataset Overview
The dataset is composed of the following tables:

Products: Information about banking products.

prod_id (VARCHAR): Unique identifier for each product.
prod_name (VARCHAR): Name of the product.
Employees: Details of bank employees.

Emp_ID (VARCHAR): Unique identifier for each employee.
Emp_Name (VARCHAR): Name of the employee.
Salary (FLOAT): Salary of the employee.
gender (VARCHAR): Gender of the employee (M/F).
Customers: Information about bank customers.

Customer_ID (VARCHAR): Unique identifier for each customer.
First_Name (VARCHAR): First name of the customer.
Last_Name (VARCHAR): Last name of the customer.
Phone (BIGINT): Phone number of the customer.
Address (VARCHAR): Address of the customer.
dob (DATE): Date of birth of the customer.
Accounts: Bank accounts information.

Account_No (BIGINT): Unique identifier for each account.
Balance (INT): Current balance of the account.
Account_Status (VARCHAR): Status of the account (Active/Inactive/Suspended/On hold).
Date_of_Opening (DATE): Date when the account was opened.
Transactions: Records of transactions.

Transaction_ID (INT): Unique identifier for each transaction (auto-generated).
Transaction_Date (DATE): Date of the transaction.
Transaction_Amount (FLOAT): Amount of the transaction.
Credit_Debit_Flag (VARCHAR): Indicates if the transaction is a credit or debit (C/D).
Account_No (BIGINT): Foreign key linking to the Accounts table.
Customer_Accounts: Mapping between customers and their accounts.

Customer_ID (VARCHAR): Foreign key linking to the Customers table.
Account_No (BIGINT): Foreign key linking to the Accounts table.
prod_id (VARCHAR): Foreign key linking to the Products table.
