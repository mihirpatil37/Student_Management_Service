# Students Management System

A desktop application built with **PyQt6** that allows users to manage student records including adding, editing, searching, and deleting entries stored in a **SQLite** database.

---

## Screenshot

![Students Management System UI](Student%20Management%20System..PNG)

---

## Features

- **Search Students** by name
- **Add Students** with name, course, and mobile number
- **Edit Student Records** directly from the table
- **Delete Records** with confirmation
- **View All Records** in a dynamic table
- **About Dialog** for application information
- Simple and responsive **GUI**

---

## Project Structure


```
├── main.py # Main application code
├── icons/ # Folder for action icons (add.png, search.png)
├── database.db # SQLite database (auto-created)
├── Student Management System..PNG # Screenshot image
└── README.md # Project documentation
```

---

## Requirements

- Python 3.7+
- PyQt6

---

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/students-management-system.git
    cd students-management-system
    ```

2. Create a virtual environment (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate      # On Unix or MacOS
    venv\Scripts\activate         # On Windows
    ```

3. Install dependencies:
    ```bash
    pip install PyQt6
    ```

4. Run the application:
    ```bash
    python main.py
    ```

---

## Database

The SQLite database is named `database.db` and contains a single table:

```sql
CREATE TABLE students (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    name TEXT NOT NULL,
    course TEXT NOT NULL,
    mobile TEXT NOT NULL
);
```
## How to Use
- Use the File > Add Student menu or toolbar to add new entries.
- Click on a row in the table to enable Edit and Delete buttons in the status bar.
- Use the Edit button to update the selected record.
- Use the Delete button to remove the selected student.
- Use the Edit > Search menu to find a student by name.
- Use Help > About to view application credits.

## License
This project is provided for educational purposes as part of "The Python Mega Course". Feel free to modify and reuse.

## Acknowledgments
Created as part of "The Python Mega Course" tutorial by Ardit Sulce.
