# Library Database Management System

## Overview
This project implements a relational database schema for a library management system using SQL. It enables efficient management of books, authors, clients, and borrowing transactions, providing a solid foundation for building a library management application.

## Features
- **Author Management**: Store and manage author details, including name and nationality.
- **Book Management**: Keep track of books, their titles, genres, and associated authors.
- **Client Management**: Manage client information, including personal details and occupation.
- **Borrowing System**: Track borrowing transactions, including borrowing dates and associated clients and books.
- **Indexing**: Create indexes on key fields for improved search performance.

## Database Schema
The following tables are created in the database:

1. **Author**
   - `AuthorID` (Primary Key)
   - `AuthorFirstName`
   - `AuthorLastName`
   - `AuthorNationality`

2. **Book**
   - `BookID` (Primary Key)
   - `BookTitle`
   - `AuthorID` (Foreign Key)
   - `Genre`

3. **Client**
   - `ClientID` (Primary Key)
   - `ClientFirstName`
   - `ClientLastName`
   - `ClientDOB`
   - `Occupation`

4. **Borrower**
   - `BorrowID` (Primary Key)
   - `ClientID` (Foreign Key)
   - `BookID` (Foreign Key)
   - `BorrowDate`
