Code Generator

Code Generator is a software tool designed to automatically generate code based on user input or database structure. Its primary goal is to save development time and reduce manual coding errors.

Features
1. Class Generation

Automatically creates a class for each database table.

Generates properties for each column in the table.

Example: Table Users → Class clsUsers with ID, Name, Email.

2. Data Access Layer (DAL) Functions

Provides core functions for each table:

Insert

Update

Delete

GetAll

FindByID

FindByName

Uses SQL parameters to prevent SQL injection.

Users can choose which functions to generate.

3. Business Layer (BL) Functions

Functions include data validation before sending to DAL.

Example: Verify email format or ensure required fields are not empty.

Connects DAL with the Presentation Layer (PL).

4. Validation Functions

Validates input data:

5. SQL Query Generation

Automatically generates SQL queries:

SELECT * FROM TableName

INSERT INTO TableName ...

UPDATE TableName SET ... WHERE ...

DELETE FROM TableName WHERE ...

6. Database Generation

With tables: Generate a new database from scratch, including:

CREATE DATABASE

CREATE TABLE

CREATE PRIMARY/FOREIGN KEYS

Without tables: Connect to an existing database and extract tables


