Library Management System (Console-Based Java Application)
📌 Description

This project is a console-based Library Management System implemented in Java.
The system manages books, members, and borrowing operations entirely in memory without using any database or file storage.

It demonstrates Low-Level Design (LLD) concepts such as:

Object-Oriented Programming

Separation of concerns using packages

Data management using collections like HashMap and ArrayList

Menu-driven console interaction

🏗 Project Structure
LibraryZoho
│
└── src
    │
    ├── model
    │     ├── Book.java
    │     ├── Member.java
    │     └── BorrowRecord.java
    │
    ├── service
    │     └── LibraryService.java
    │
    └── main
          └── Main.java
Package Description
Package	Purpose
model	Contains entity classes like Book, Member, and BorrowRecord
service	Contains business logic for library operations
main	Entry point of the application
⚙ Functional Features
1️⃣ Add Book

Adds a new book to the library.

Each book contains:

Book ID (Unique)

Title

Author

Number of copies

2️⃣ Register Member

Registers a new library member.

Each member contains:

Member ID (Unique)

Name

3️⃣ Borrow Book

A member can borrow a book if:

Copies are available

The member has borrowed fewer than 3 books

The same book is not borrowed twice by the same member

Borrow details recorded:

Borrow Date

Due Date (14 days)

4️⃣ Return Book

When a book is returned:

Available copies increase

Fine is calculated if overdue

Fine Rule:

Fine = ₹2 per overdue day
5️⃣ Search Book

Search books using:

Title

Author

Supports partial keyword matching.

Example:

Input: java
Output: Java Programming
6️⃣ Member Report

Displays all books currently borrowed by a member.

Shows:

Book title

Borrow date

Due date

7️⃣ Book Report

Displays which members currently borrowed a particular book.

8️⃣ Top Borrowers

Displays members sorted by total number of books borrowed (descending).

OUTPUT:

<img width="603" height="419" alt="image" src="https://github.com/user-attachments/assets/a83fbf53-3354-4925-8e22-686ff64b24e4" />

<img width="515" height="337" alt="image" src="https://github.com/user-attachments/assets/1828e6a1-00a7-46ae-8564-10754e9bc0da" />

<img width="631" height="346" alt="image" src="https://github.com/user-attachments/assets/a84d8eda-dfe2-4d34-9821-1dc3e0c9d2e4" />

<img width="510" height="275" alt="image" src="https://github.com/user-attachments/assets/b270ecb0-4840-4221-9018-a575be8a32b6" />



