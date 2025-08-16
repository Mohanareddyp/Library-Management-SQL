# Library Management System (C Version)

This is a **console-based Library Management System** written in C.  
It allows adding, listing, removing, and issuing books using simple file handling (`books.txt` and `issue.txt`).

## 📌 Features
- **Add Book** – Add new books with ID, title, author, and date of entry.  
- **Books List** – Display all available books in tabular format.  
- **Remove Book** – Delete a book record by its ID.  
- **Issue Book** – Issue a book to a student by entering student details.  
- **Issued Books List** – View all books issued along with student info and date.  

## 📂 File Handling
- `books.txt` → Stores all available book records.  
- `issue.txt` → Stores issued book records with student details.  
- `temp.txt` → Used internally when removing books.  

## ⚙️ How It Works
- The system uses **C structures**:
  - `struct books` – to store book details.  
  - `struct student` – to store issued book and student details.  
- Records are stored persistently in text files using `fwrite()` and `fread()`.  
- The program runs in a menu-driven loop until the user exits.

## ▶️ How to Run
1. Save the source file as `lib.c`.  
2. Compile using:
   ```bash
   gcc lib.c -o library
