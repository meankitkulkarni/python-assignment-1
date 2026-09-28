# Assignment Report

## Student Record Management System

### Submitted By

**Name:** Ankit Sachin Kulkarni  
**Roll No.:** 39  
**Course:** Master of Computer Applications (MCA)  
**Subject:** Python Programming  

---

## 1. Introduction

The Student Record Management System is a menu-driven Python application developed to manage basic student information. The program allows the user to add, view, search, update and delete student records.

The project is designed using core Python concepts and stores data in a JSON file. Because the records are stored in a file, the information remains available even after the program is closed and opened again.

---

## 2. Objective

The main objective of this project is to understand and practically apply the fundamental concepts of Python programming in one complete application.

The project demonstrates:

- Variables and data types
- Lists and dictionaries
- Conditional statements
- Loops
- Functions
- File handling
- JSON data storage
- Exception handling
- Input validation
- Regular expressions
- CRUD operations

---

## 3. Problem Statement

Managing records manually can become difficult when the number of students increases. Searching, editing or deleting a particular record may take time.

This project provides a simple console-based solution where student records can be managed using a numbered menu.

---

## 4. Scope of the Project

The system stores the following information for every student:

- Student ID
- Name
- Course
- Semester
- Email
- Phone number
- Marks

The system supports ten sample records and can also accept additional records from the user.

---

## 5. Functional Requirements

### 5.1 Add Student

The user can enter a student's name, course, semester, email, phone number and marks.

A unique Student ID such as `S001`, `S002` and `S003` is generated automatically.

### 5.2 View Students

The user can display all available student records.

The total number of students is also displayed.

### 5.3 Search Student

A student can be searched using:

1. Student ID
2. Full or partial name

Name search is case-insensitive.

### 5.4 Update Student

The user can modify an existing student's details.

If a field is left blank, the existing value is retained.

### 5.5 Delete Student

A student can be deleted using the Student ID.

The application asks for confirmation before deleting the record.

### 5.6 Student Statistics

The program calculates:

- Total number of students
- Average marks
- Highest marks
- Lowest marks

### 5.7 Persistent Storage

All records are stored inside `records.json`.

Changes made through Add, Update or Delete are saved automatically.

---

## 6. Input Validation

The application performs validation to reduce incorrect data.

### Email

A regular expression is used to check the basic structure of the email address.

### Phone Number

The phone number must contain exactly 10 digits.

### Semester

Only values from 1 to 6 are accepted.

### Marks

Marks must be between 0 and 100.

### Empty Input

Important text fields such as name and course cannot be empty.

---

## 7. Data Structure Used

The application stores all records in a Python list.

Each individual student is represented using a dictionary.

Example:

```python
{
    "student_id": "S010",
    "name": "Ankit Sachin Kulkarni",
    "course": "MCA",
    "semester": 1,
    "email": "ankit.kulkarni@example.com",
    "phone": "9000000010",
    "marks": 87
}
```

So the overall structure is:

```text
List
 ├── Student Dictionary 1
 ├── Student Dictionary 2
 ├── Student Dictionary 3
 └── ...
```

---

## 8. Main Functions

### `load_records()`

Reads student data from `records.json`.

### `save_records(records)`

Writes the current list of records to `records.json`.

### `get_next_student_id(records)`

Generates the next Student ID automatically.

### `add_student(records)`

Collects validated student information and adds a new record.

### `view_students(records)`

Displays all available student records.

### `search_student(records)`

Searches by Student ID or student name.

### `update_student(records)`

Allows modification of an existing record.

### `delete_student(records)`

Deletes a student after confirmation.

### `show_statistics(records)`

Calculates total students, average marks, highest marks and lowest marks.

### `display_menu()`

Displays the main menu.

### `main()`

Controls the complete application flow.

---

## 9. Program Flow

```text
Start
  ↓
Load Student Records
  ↓
Display Menu
  ↓
Read User Choice
  ↓
Perform Selected Operation
  ↓
Save Data if Modified
  ↓
Return to Menu
  ↓
Exit
```

---

## 10. CRUD Operations

CRUD stands for:

- **Create** – Add a new student
- **Read** – View or search student records
- **Update** – Modify an existing student
- **Delete** – Remove an existing student

The project demonstrates all four CRUD operations.

---

## 11. Exception Handling

`try` and `except` blocks are used so that incorrect input or file problems do not immediately crash the application.

Examples include:

- Invalid numeric values
- Invalid marks
- Invalid semester
- Missing JSON file
- Corrupted JSON data
- File reading or writing errors
- Keyboard interruption

---

## 12. Sample Students

The sample JSON database contains ten MCA students:

1. Jitesh Vishwakarma
2. Prajwal Bhosale
3. Vrushabh Sonawane
4. Rishikesh Hedwe
5. Param Gala
6. Sneha Patil
7. Sanika Patil
8. Deeya Mathur
9. Om Patil
10. Ankit Sachin Kulkarni

The emails, phone numbers and marks used in the supplied sample data are demonstration values only.

---

## 13. Advantages

- Simple and easy to understand
- No external Python libraries required
- Data remains saved after closing the application
- User input is validated
- Code is divided into separate functions
- All major CRUD operations are included
- Suitable for demonstrating basic Python programming concepts

---

## 14. Limitations

- The application runs only in the console.
- It uses a local JSON file instead of a database server.
- It does not provide login or user authentication.
- The statistics are basic.
- It is designed for educational use rather than large-scale deployment.

---

## 15. Future Improvements

The project can later be extended by adding:

- Graphical User Interface using Tkinter
- MySQL or SQLite database
- Login system
- Student attendance
- Subject-wise marks
- Grade calculation
- Export to CSV
- Sorting and filtering
- Web-based interface

---

## 16. Conclusion

The Student Record Management System successfully demonstrates how basic Python programming concepts can be combined to create a useful application.

Through this project, concepts such as lists, dictionaries, loops, conditions, functions, JSON file handling, exception handling, regular expressions and CRUD operations are used together in a practical way.

The project also shows the importance of modular programming, input validation and persistent data storage.

---

**Submitted By:**  
**Ankit Sachin Kulkarni**  
**Roll No. 39**  
**MCA**
