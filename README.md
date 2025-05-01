# 📚 JournalEase - Library Management System

**JournalEase** is a modern Library Management System (LMS) built to streamline the management of books, track borrowing records, and enhance the user experience for both librarians and patrons. It offers an intuitive interface and robust backend using Python, Tkinter, and MySQL.

## 📌 Key Features

- Add Book: Add new books to the library collection with ease.
- Search Book: Quickly find books by Title, Author, or ISBN.
- Issue Book: Efficiently issue books to library users.
- Book Holder: Keeps track of who currently has a specific book.
- Return Book: Mark books as returned and update availability.
- View All Books: Display a complete list of books in the system.
- Update and Delete Book Records

## 🛠️ Technologies Used

- **Python**: Backend logic implementation using a versatile and readable language.
- **Tkinter**: GUI development for a clean and user-friendly desktop interface.
- **MySQL**: Relational database to manage books, users, and transactions efficiently.
- **PyMySQL**: Interface between Python and MySQL database.

## 📷 UI Snapshots

![All Books](https://github.com/user-attachments/assets/b443194a-5c95-4e97-a1bd-962d3124df44)
![Add Book](https://github.com/user-attachments/assets/0eb1baa0-f7f5-4940-8f39-669114c73d55)
![Search Book 2](https://github.com/user-attachments/assets/c25bb3e8-cd1b-4a56-96a0-f6f4d2603d5f)
![Search Book 1](https://github.com/user-attachments/assets/eb2b349d-790b-437a-b075-5a4b6dbb6594)
![Issue Book](https://github.com/user-attachments/assets/3775eb1e-47e9-4371-8241-05759e34d847)
![Return book 2](https://github.com/user-attachments/assets/d9e292bc-f625-4526-874f-e9a80eb3acd1)
![Return Book 1](https://github.com/user-attachments/assets/8453c3c8-6d64-4316-add4-6e9206265522)

## 📁 Project Structure

- main.py : Main logic and GUI functionality
- custom.py : Font and color configuration
- credentials.py : MySQL username and password (user-defined)

## 🛢️ Database

<pre>CREATE DATABASE library_management;</pre>
<pre>CREATE TABLE book_list(
	book_id VARCHAR(10) NOT NULL,
	book_name VARCHAR(50) NOT NULL,
	author VARCHAR(50) NOT NULL,
	edition VARCHAR(10) NOT NULL,
	price Int(6) NOT NULL,
	qty Int(4) NOT NULL,
	PRIMARY KEY ( book_id )
); </pre>
<pre>CREATE TABLE borrow_record(
	book_id VARCHAR(10) NOT NULL,
	book_name VARCHAR(50) NOT NULL,
	stu_roll VARCHAR(15) NOT NULL,
	stu_name VARCHAR(50) NOT NULL,
	course VARCHAR(10) NOT NULL,
	subject VARCHAR(30) NOT NULL,
	issue_date date NOT NULL,
	return_date date NOT NULL
);</pre>


> Developed as a part of the OOP Lab Project at Daffodil International University.
