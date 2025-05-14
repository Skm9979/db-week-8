# db-week-8

[14/05, 12:35 am] : Skm9979# Library Management System 📚

Project Title

Library Management System 🔐

Description

A 📁 MySQL-based relational database schema for managing a library’s core operations, including:

👨‍🎓 Authors: Store information about book authors.

📖 Books: Track book metadata (ISBN, title, publisher, publication date).

📚 Categories: Organize books into genres with a many-to-many relationship.

👤 Patrons: Maintain library member profiles and contact details.

💼 Staff: Manage librarian accounts and roles.

⏳ Loans: Record book checkouts, due dates, and returns.

🗲️ Reservations: Allow patrons to place holds on books.

This schema ✨ enforces data integrity through primary keys, foreign keys, NOT NULL, and UNIQUE constraints, and models 1-1, 1-M, and M-M relationships.

📊 Entity Relationship Diagram (ERD) – Library Management System 📘 Project Context This ERD visualizes the relational structure of the Library Management System database. It outlines how key entities such as books, authors, patrons, and staff interact with one another, enforcing data integrity through constraints like primary keys, foreign keys, and relationship cardinalities.

🧱 Entities & Relationships The following entities are included:

Author: Holds information about book writers.

Book: Contains metadata for each book, with a foreign key to Author.

Category: Defines book genres. Books can belong to multiple categories.

BookCategory: A junction table for the many-to-many relationship between Book and Category.

Patron: Library members who borrow and reserve books.

Staff: Employees or librarians who manage transactions.

Loan: Records when a book is checked out by a patron and handled by staff.

Reservation: Tracks holds placed on books by patrons.

🔐 Keys & Constraints ✅ Primary Keys (PK): Every entity includes an id column as the primary key.

🔗 Foreign Keys (FK): Implemented for all dependent relationships to maintain referential integrity.

🔒 NOT NULL / UNIQUE constraints ensure data consistency and prevent duplicates.

📌 Cardinalities 1:N between Author and Book

M:N between Book and Category via BookCategory

1:N between Patron and Loan

1:N between Book and Loan

1:N between Staff and Loan

1:N between Patron and Reservation
