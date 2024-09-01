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

## How to Run the Process

### Step 1: Download the CSV Files

Download the required CSV files as a ZIP archive from this link:

[Download CSV Files](https://github.com/Saikrishnamotaparthi/Library-Management-System-in-R/blob/6eb879e3548d7d9b41a7b1ef81ab0e94cda2be11/CSV%20FILES.zip)

### Step 2: Extract the CSV Files

Extract the contents of the ZIP archive to a folder on your computer. Ensure that the following files are present:

- `students.csv`
- `engineering_books.csv`
- `CART.csv`
- `checkout.csv`

### Step 3: Update File Paths in the Code

After extracting the files, update the file paths in the `get_file_paths()` function in the R script to reflect the location where you extracted the CSV files. For example:

```r
get_file_paths <- function() {
  students_file <- "C:/path/to/your/extracted/files/students.csv"
  books_file <- "C:/path/to/your/extracted/files/engineering_books.csv"
  cart_file <- "C:/path/to/your/extracted/files/CART.csv"
  checkout_file <- "C:/path/to/your/extracted/files/checkout.csv"
  
  return(list(students_file=students_file, books_file=books_file, cart_file=cart_file, checkout_file=checkout_file))
}



