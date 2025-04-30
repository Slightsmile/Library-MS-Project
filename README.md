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
