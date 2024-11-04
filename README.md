
# 📚 Library Book Management System

Welcome to the Library Book Management System! This program, written in C, allows you to manage a collection of books with functionalities like tracking availability, monitoring borrow counts, and identifying popular books. It’s an ideal solution for managing a small library or personal book collection efficiently.

## 🚀 Features

- **📖 Add New Books**: Easily add new books with essential details like name, author, and initial availability.
- **🔄 Track Availability**: The system maintains the availability status of each book to ensure accurate borrowing information.
- **📊 Borrow Count Tracking**: Each time a book is borrowed, the system records it, allowing for insights into popular books.
- **🏆 Identify Top Books**: Quickly find the most-borrowed books in your collection for better inventory management.

## 📁 File Structure

- **main.c**: The main program file containing all functions and logic for book management, including memory allocation, borrowing, availability checks, and user interaction prompts.

## 🛠️ Getting Started

To use this program, you’ll need to compile and run it on a C compiler. Follow these steps to get started:

### Compilation and Execution

1. **Compile** the program:
   ```bash
   gcc -o library_system main.c
   ```
2. **Run** the compiled executable:
   ```bash
   ./library_system
   ```

### Program Workflow

1. **Welcome Prompt**: The program welcomes you and provides options to add books, borrow books, or check their availability.
2. **Add Book**: Input book details such as the name and author to add it to your collection.
3. **Borrow**: Borrow a book to update its status and borrow count automatically.
4. **Finalize**: At the end of your session, the program displays all book details along with borrow statistics for reference.

## 📂 Core Functions

The main functions in this program include:

- **`Book* new_book(const char *name, const char *author, Book *books[BOOK_NUM])`**:
  - Creates a new book by allocating memory and setting initial values.
  - Parameters: Book name, author name, and the book array.
  - Returns a pointer to the newly created book.

- **`void string_print(char *str)`**:
  - A helper function for formatted output of strings.

- **`void print_book(Book book)`**:
  - Displays the details of a book, including its name and author.
  - Parameters: A `Book` structure.

### Example Commands

Here’s what an example session might look like:

1. **Adding a New Book**
   - When prompted to add a new book, enter:
     ```text
     Name: "To Kill a Mockingbird"
     Author: "Harper Lee"
     ```
   - The system sets an initial availability count and starts tracking borrow count.

2. **Borrowing a Book**
   - To borrow a book, specify the book’s name:
     ```text
     Borrowed: "To Kill a Mockingbird"
     ```
   - The system updates the availability count and increases the borrow count.

3. **Viewing Top Borrowed Books**
   - The program keeps track of how often each book is borrowed, allowing you to see which books are most popular.

## ⚠️ Error Handling

The program includes basic error handling to ensure smooth execution:

- **Memory Allocation Errors**: If memory allocation fails while creating a new book, the program will display an error message and free any previously allocated memory to prevent leaks.

Thank you for checking out the Library Book Management System! Enjoy organizing your collection and tracking your most popular reads. 📖
