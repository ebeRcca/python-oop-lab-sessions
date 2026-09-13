# OOP Practice Examples

## Overview

This folder contains two Python programs I wrote while learning the basics of object‑oriented programming (OOP). Each program uses simple classes, attributes, and methods to build a basic system. 

## Programs Included

### 1. Banking System
**File:** `simple_banking_system.py`

A simple program that allows a user to:
- create an account  
- deposit money  
- withdraw money  
- check their balance  

It uses a basic `Account` class with attributes for storing balance and methods for updating it.

### 2. Library System
**File:** `simple_library_system.py`

A small program that lets a user:
- add books to the library  
- register members  
- borrow and return books for members 

It uses classes such as `Book`, `Member`, and `Library` to organise the system’s data and actions.

## Purpose

I selected these programs to explain how software design principles are demonstrated in my code. Both programs provide clear examples of basic OOP structure and how classes interact within a system.

## Software Design Principles Demonstrated

### Modularity
Modularity refers to breaking a program into smaller, independent modules. In these programs, each module has a clear responsibility. For example the classes demonstrate modularity: `Account` manages balance information, `Book` stores single book details, and `Member` stores member information. This separation makes the system easier to understand and maintain.

### Cohesion
Cohesion describes how closely related the elements of a module are. In these programs, classes such as `Account`, `Book`, and `Member` show high cohesion because the attributes and methods inside each class relate to the same area of responsibility. The `Library` class has lower cohesion because it combines several responsibilities such as managing books, members, and borrowing, although all of these still relate to the overall purpose of coordinating the library system. This is common in small beginner programs where one class handles the main system operations.

### Coupling
Coupling refers to how dependent modules are on each other. These programs demonstrate low coupling because classes interact through simple method calls rather than accessing each other’s internal data. The `Library` class communicates with `Book` and `Member` objects by calling their methods, which reduces interdependence and makes the system easier to update or modify.

### Abstraction
Abstraction hides unnecessary details and exposes only what is needed. Methods such as `deposit()`, `withdraw()`, `borrow_book()`, and `return_book()` provide clear actions without requiring the user to understand how the data is stored or updated internally. This keeps the interface simple and reduces complexity for anyone using the program.

### Encapsulation
Encapsulation bundles data and behaviour together while restricting direct access to internal details. Attributes such as `balance` or `status` are stored inside classes and changed only through methods. This prevents accidental modification and ensures that each class controls how its own data is managed.

### KISS (Keep It Simple)
The KISS principle encourages keeping code simple and avoiding unnecessary complexity. These programs follow KISS by using straightforward logic, clear method names, and easy‑to‑follow class structures. Each action, such as borrowing a book or depositing money, is implemented in a simple, readable way.

### Separation of Concerns
Separation of Concerns means dividing a system so each class is responsible for a different part of the overall functionality. In both programs, each class has a clear role: `Account` manages money, `Book` stores book information, `Member` keeps track of member details, and `Library` coordinates borrowing, returning, and managing the collection. This shows how each class focuses on its own responsibility without overlapping with others.
  
### Reusability
Reusability refers to designing classes that can be used in other programs. Classes such as `Account`, `Book`, and `Member` are reusable because they contain self‑contained logic and do not depend on specific program details. They could be used in other banking or library systems with little modification.
