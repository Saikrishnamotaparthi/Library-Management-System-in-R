# Library Management System in R

This is a simple Library Management System implemented in R that allows you to manage students, books, and checkouts. The system uses CSV files for data storage and provides a command-line interface for managing library operations.

## Project Structure

- **students.csv**: Stores student profiles (StudentID, Name, Email).
- **engineering_books.csv**: Stores book information (BookID, Title, Author, Quantity).
- **CART.csv**: Temporarily stores items that students want to check out.
- **checkout.csv**: Logs all book checkouts (StudentID, BookID, Title, Quantity).

## Features

1. **Add Student**: Add a new student profile to the system.
2. **Show Books**: Display all available books along with their quantities.
3. **Add Book**: Add new books to the library inventory.
4. **Add to Cart**: Add books to a student's cart for checkout.
5. **Checkout**: Process checkout, update book quantities, and log the transaction.
6. **Show Checked-Out Books**: View the list of books checked out by a particular student.

## How It Works

- The system reads and writes data to CSV files stored in the specified file paths.
- Each feature is accessible through a menu-based interface, allowing users to interact with the system.
- Before performing any action, the system checks for the existence of necessary files and creates them if they do not exist.

## Installation

1. Make sure you have R installed on your system.
2. Clone the repository and navigate to the project directory.
3. Install the necessary package:

   ```R
   install.packages("readr")
