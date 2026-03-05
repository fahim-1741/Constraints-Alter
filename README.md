# Constraints-Alter
This SQL project demonstrates a Library Management System database. It illustrates the use of core database concepts such as primary keys, foreign keys, unique constraints, check constraints, default values, and enumerated types (ENUM) to maintain data integrity and consistency.

The database manages members, books, and borrow records in a structured and secure way.

Key Principles Demonstrated

The project highlights several important principles in database design:

Data Integrity

Uses primary keys to uniquely identify members, books, and borrow records.

Ensures unique emails and ISBN numbers with UNIQUE constraints.

Validates Age (>=12) and Price (>=0) using CHECK constraints.

Referential Integrity

Uses foreign keys in the BORROW table to link members and books.

Prevents inconsistent borrow records if a member or book does not exist.

Controlled Defaults

Phone defaults to 'N/A' if not provided.

Availability defaults to 'AVAILABLE' for new books.

Restricted Values

Availability is restricted using ENUM('AVAILABLE','BORROWED').

Prevents invalid data from being entered into the database.

Program Demonstration Steps

The database execution demonstrates the benefits of proper table design:

Database Setup

library_lab is created and used for all operations.

Table Creation

Three tables are created: MEMBER, BOOK, and BORROW.

Constraints ensure data integrity and consistency.

Data Insertion

Sample members and books are added with valid data.

Borrow transactions are recorded in the BORROW table.

Validation Checks

Invalid data such as age below 12 or negative book price is rejected.

Borrow records cannot reference non-existent members or books.

Data Access

All data can be retrieved safely using SELECT queries.

Foreign keys ensure that all borrow records reference valid members and books.
