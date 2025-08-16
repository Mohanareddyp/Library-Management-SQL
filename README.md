# Library Management System (SQL Version)

This project is a database-driven Library Management System, originally converted from a C program that used text files.  
It demonstrates how file-based storage can be redesigned using **SQL schema** and queries.

## Features
- Add new books  
- List available books  
- Delete books  
- Issue books to students  
- View issued books with student details  

## Database Schema
- `Books` table → Stores book details (ID, Name, Author, Date Added)  
- `IssuedBooks` table → Stores issued records linked to book IDs  

## How to Use
1. Import `library_management.sql` into MySQL/SQLite.  
2. Run the provided queries to manage the library.  

## Example Queries
```sql
INSERT INTO Books (id, bookName, authorName, addedDate)
VALUES (1, 'C Programming', 'Dennis Ritchie', CURDATE());

SELECT * FROM Books;
