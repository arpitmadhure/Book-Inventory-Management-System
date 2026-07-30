# 📚 Book Inventory Management System

A simple Book Inventory Management System developed using **Python** and **MySQL**. The application enables users to manage book records efficiently through a command-line interface, supporting inventory management operations such as adding, searching, updating, and viewing books.

## Overview

This project provides a database-driven solution for managing book inventories. It integrates Python with MySQL to perform CRUD operations while maintaining a structured and user-friendly workflow.

## Key Features

- Create the books table automatically if it does not already exist.
- Add new books to the inventory.
- Search books using Title, Author, or ISBN.
- Update the quantity of existing books.
- Display the complete inventory.
- Simple and interactive command-line interface.

## Technologies Used

- Python
- MySQL
- MySQL Connector for Python
- Exception Handling

## Prerequisites

Before running the project, ensure you have:

- Python 3 or later
- MySQL Server
- MySQL Connector for Python

Install the required package:

```bash
pip install mysql-connector-python
```

## Database Setup

### Step 1: Create the Database

```sql
CREATE DATABASE book_inventory;
```

### Step 2: Configure Database Credentials

Update the database connection inside `book_inventory.py`.

```python
mydb = mysql.connector.connect(
    host="localhost",
    user="root",
    password="your_password",
    database="book_inventory"
)
```

## Running the Project

Start MySQL and execute:

```bash
python book_inventory.py
```

Then follow the on-screen menu to manage the inventory.

## Usage

### Add a Book

Enter:

```
Title, Author, ISBN, Quantity
```

### Search Books

Search using:

- Title
- Author
- ISBN

### Update Quantity

Provide:

- Book ID
- New Quantity

### View Inventory

Displays all books currently stored in the database.

### Exit

Select **Option 5** to close the application.

## Future Enhancements

- Graphical User Interface (GUI)
- User Authentication
- Inventory and Availability Reports

## License

This project is open-source and free to use.

## Author

**Arpit Madhure**

Contributions and suggestions are always welcome.
