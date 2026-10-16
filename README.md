# Gradebook Management System - Section D

# Overview

This section of the Gradebook Management System focuses on modularizing the program using functions.
The aim is to improve code organization, readability, reusability and maintainability by breaking repetitive tasks into separate functions.

# The program allows users to:

* Add student records

* Calculate student averages

* Display individual student records

* Display a summary of all students 

* Search for students

* Update student grades

* View grades by subject

* Handle invalid user input without crashing

# Objective
Refactor the Gradebook Management System by creating reusable functions for common tasks and implementing proper error handling.

Functions Implemented
1. get_grade(subject)

Purpose
* Accepts a grade for a subject.
* Validates the grade.
* Ensures grades are between 0 and 100.
* Handles non-numeric input using try/except.

2. get_grade("Math")
calculate_average(math, english, science)

Purpose

* Calculates and returns the average grade for a student.
  
Formula

average = (math + english + science) / 3
add_student(students_dict)

Purpose

* Adds a new student to the dictionary.
* Collects grades for Mathematics, English, and Science.
* Stores grades using a nested dictionary structure.
  
Example Structure

students_dict = {
    "John": {
        "Math": [80],
        "English": [75],
        "Science": [90]
    }
}
3. display_student(students_dict, student_name)

Purpose

Displays an individual student's:
* Name
* Subject grades
* Average grade

4. display_summary(students_dict)

Purpose

* Displays a complete summary of all student records.
* Displays each student's grades and calculated average.
  
5. update_student(students_dict)

Purpose

* Searches for a student by name.
* Updates existing grades.
* Validates user input before updating records.

6. search_student(students_dict)

Purpose

* Searches for a student in the dictionary.
* Displays the student's grades and average.

7. view_subject_grades(students_dict)

Purpose

* Allows the user to select a subject.
* Displays grades for that subject across all students.

Available Subjects:
* Math
* English
* Science

Data Structure Used:
The program uses a nested dictionary structure.

Example

students_dict = {
    "Mary": {
        "Math": [85],
        "English": [90],
        "Science": [88]
    }
}

# Advantages
* Student names are used as keys.
* Subjects are stored as keys.
* Grades are stored in lists.
* Records can be searched and updated efficiently.
* Error Handling
* The program uses try/except blocks to prevent runtime errors and improve user experience.

# Non-Numeric Input

Input

Enter Math grade: abc

Output

Invalid input. Please enter a numeric grade.

Invalid Grade Range

Input

Enter Math grade: 150

Output

Grade must be between 0 and 100.

Missing Student Name

Input

Enter student name:

Output

Student name cannot be empty.

Non-Existent Student

Input

Enter student name to search: Peter

Output

Student not found.

# Program Menu

The system provides the following options:

* Add Student
* Update Student
* Search Student
* View Subject Grades
* Display Student Summary
* Exit

# Key Concepts Demonstrated

* Functions
  
* Dictionaries
  
* Nested Dictionaries
  
* Lists
  
* Reusable Code
  
* Input Validation
  
* Exception Handling
  
* Searching Records
  
* Updating Records
  
* Average Calculations

# Conclusion
Section D improves the Gradebook Management System by introducing functions to reduce code repetition and improve organization.
Tasks such as adding students, calculating averages, displaying records, searching, and updating data are handled through reusable functions.
Input validation and error handling have also been included to make the system more reliable, maintainable and user-friendly.


This project was developed and tested using:

IDE: PyCharm

Programming Language: Python

Python Version: 3.14.7

Operating System: Windows

The application was executed and tested within the PyCharm development environment.
