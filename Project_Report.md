# Project Report: To-Do List Application

## 1. Project Title
**To-Do List Application Using Python**

## 2. Introduction
The To-Do List Application is a simple command-line Python project designed to help users manage a list of tasks. The program allows the user to add tasks, view existing tasks, delete tasks, and exit the application.

The project demonstrates basic Python programming concepts such as lists, loops, conditional statements, user input, list methods, and enumeration.

## 3. Objective
The main objectives of this project are:
- To create a simple task-management application.
- To understand how Python lists can store and manage multiple tasks.
- To implement a menu-driven program.
- To practice conditional statements and loops.
- To use list methods such as `append()` and `pop()`.
- To provide basic validation for invalid choices and task numbers.

## 4. Technologies Used
- **Programming Language:** Python
- **Interface:** Command-line / console
- **Data Structure:** Python list

## 5. Features
The application provides four main options:

1. **Add Task** – Allows the user to enter a new task and adds it to the task list.
2. **View Tasks** – Displays all currently stored tasks with serial numbers.
3. **Delete Task** – Allows the user to select a task number and remove that task.
4. **Exit** – Terminates the application.

## 6. Working of the Project
At the beginning, an empty list named `tasks` is created. The program then repeatedly displays a menu using a `while True` loop.

When the user selects:
- **Option 1:** The entered task is added using `tasks.append(task)`.
- **Option 2:** The program checks whether the list is empty. If not, it displays the tasks using `enumerate()`.
- **Option 3:** The program displays the tasks and asks for a task number. If the number is valid, `pop()` removes the corresponding task.
- **Option 4:** The program prints a goodbye message and exits the loop.
- **Any other option:** The program displays an invalid-choice message.

The uploaded source code implements these menu options and task operations. fileciteturn0file0L3-L14

## 7. Python Concepts Used

### 7.1 List
The program uses a Python list to store tasks:

```python
tasks = []
```

### 7.2 `append()`
The `append()` method adds a new task to the end of the list. fileciteturn0file0L12-L15

### 7.3 `len()`
The `len()` function is used to check whether there are any tasks and to validate a task number. fileciteturn0file0L17-L19

### 7.4 `enumerate()`
The `enumerate()` function displays tasks with numbers starting from 1. fileciteturn0file0L21-L23

### 7.5 `pop()`
The `pop()` method removes a selected task from the list. Since list indexing starts at 0, the program uses `number - 1`. fileciteturn0file0L32-L35

### 7.6 Conditional Statements
`if`, `elif`, and `else` statements are used to process the user's menu choice and validate task numbers. fileciteturn0file0L12-L45

### 7.7 Loop
A `while True` loop keeps the application running until the user chooses the Exit option. fileciteturn0file0L3-L4

## 8. Algorithm
1. Start the program.
2. Create an empty list named `tasks`.
3. Display the To-Do List menu.
4. Ask the user to enter a choice.
5. If the choice is 1, accept a task and add it to the list.
6. If the choice is 2, display all tasks if the list is not empty.
7. If the choice is 3, display tasks and ask for the task number to delete.
8. Check whether the selected task number is valid.
9. Delete the selected task if the number is valid.
10. If the choice is 4, display a goodbye message and stop.
11. Otherwise, display an invalid-choice message.
12. Repeat the menu until the user exits.

## 9. Program Flow
```text
Start
  |
Create empty task list
  |
Display Menu
  |
Enter Choice
  |
  +---- 1 ----> Enter Task -> Add Task -> Back to Menu
  |
  +---- 2 ----> Check List -> Display Tasks -> Back to Menu
  |
  +---- 3 ----> Display Tasks -> Enter Number
  |                 |
  |           Valid Number?
  |             /       \
  |           Yes        No
  |            |          |
  |       Delete Task   Show Error
  |            |          |
  |            +----> Back to Menu
  |
  +---- 4 ----> Goodbye -> End
  |
  +---- Other -> Invalid Choice -> Back to Menu
```

## 10. Sample Interaction
```text
--- TO-DO LIST ---
1. Add Task
2. View Tasks
3. Delete Task
4. Exit
Enter your choice: 1

Enter your task: Complete Python assignment
Task added!

--- TO-DO LIST ---
1. Add Task
2. View Tasks
3. Delete Task
4. Exit
Enter your choice: 2

Your Tasks:
1 . Complete Python assignment
```

## 11. Advantages
- Simple and easy to use.
- Demonstrates important Python fundamentals.
- Uses a list for efficient basic task storage.
- Menu-driven interaction is easy to understand.
- Tasks can be added, viewed, and deleted.

## 12. Limitations
- Tasks are stored only while the program is running.
- There is no permanent file or database storage.
- The program does not provide task priorities or deadlines.
- Invalid non-numeric input for the delete-task number is not explicitly handled by the current code.

## 13. Future Scope
The project can be improved by adding:
- Permanent storage using a text file or database.
- Task completion status.
- Task priorities.
- Due dates and reminders.
- Search and edit options.
- Exception handling for invalid numeric input.
- A graphical user interface.

## 14. Conclusion
The To-Do List Application is a useful beginner-level Python project that demonstrates lists, loops, conditional statements, user input, `append()`, `len()`, `enumerate()`, and `pop()`. It provides a practical example of how basic Python concepts can be combined to build a functional command-line application.
