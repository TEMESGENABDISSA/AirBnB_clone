# AirBnB Clone - The Console

  
![HolBnB clone](https://github.com/monoprosito/AirBnB_clone/blob/feature/console/hBnB.png?raw=true)
Welcome to the AirBnB clone project! (The Holberton B&B)

  # 0x00. AirBnB clone - The console
# Done by : Temesgen abdissa and yalelet dessalegn Mebrie)
# Describtion About AirBnB clone 
The 0x00 AirBnB clone, known as "The console," is an innovative group project that demonstrates the prowess of Python programming in the realm of Object-Oriented Programming (OOP). This project aims to replicate the core functionalities of the popular accommodation booking platform, Airbnb, while also serving as an educational tool for aspiring developers to delve into the intricacies of software development, design patterns, and collaborative teamwork. Through meticulously crafted Python code, the console offers users the ability to create and manage property listings, search for accommodations, handle bookings, and simulate user interactions within a command-line interface.

At the heart of the 0x00 AirBnB clone lies the strong foundation of OOP principles. Python's object-oriented features are leveraged to create modular and maintainable code, encapsulating various aspects of the application's functionality into distinct classes and objects. The project showcases the elegance of class hierarchies, inheritance, polymorphism, and encapsulation, thereby emphasizing the significance of code organization and reusability. By diving into this project, developers gain valuable experience in designing extensible systems, implementing robust error handling mechanisms, and orchestrating complex interactions between different components of the application. Through collaborative efforts, the 0x00 AirBnB clone stands as a testament to the power of Python and OOP in crafting sophisticated, interactive software solutions that mirror real-world scenarios.

# Requirements
# Python Scripts
Allowed editors: vi, vim, emacs
All your files will be interpreted/compiled on Ubuntu 20.04 LTS using python3 (version 3.8.5)
All your files should end with a new line
The first line of all your files should be exactly #!/usr/bin/python3
A README.md file, at the root of the folder of the project, is mandatory
Your code should use the pycodestyle (version 2.8.*)
All your files must be executable
The length of your files will be tested using wc
All your modules should have a documentation (python3 -c 'print(__import__("my_module").__doc__)')
All your classes should have a documentation (python3 -c 'print(__import__("my_module").MyClass.__doc__)')
All your functions (inside and outside a class) should have a documentation (python3 -c 'print(__import__("my_module").my_function.__doc__)' and python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)')
A documentation is not a simple word, it’s a real sentence explaining what’s the purpose of the module, class or method (the length of it will be verified)
# Python Unit Tests
Allowed editors: vi, vim, emacs
All your files should end with a new line
All your test files should be inside a folder tests
You have to use the unittest module
All your test files should be python files (extension: .py)
All your test files and folders should start by test_
Your file organization in the tests folder should be the same as your project
e.g., For models/base_model.py, unit tests must be in: tests/test_models/test_base_model.py
e.g., For models/user.py, unit tests must be in: tests/test_models/test_user.py
All your tests should be executed by using this command: python3 -m unittest discover tests
You can also test file by file by using this command: python3 -m unittest tests/test_models/test_base_model.py
All your modules should have a documentation (python3 -c 'print(__import__("my_module").__doc__)')
All your classes should have a documentation (python3 -c 'print(__import__("my_module").MyClass.__doc__)')
All your functions (inside and outside a class) should have a documentation (python3 -c 'print(__import__("my_module").my_function.__doc__)' and python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)')
We strongly encourage you to work together on test cases, so that you don’t miss any edge case


## Getting Started

 
**What’s a command interpreter?**

Do you remember the Shell? It’s exactly the same but limited to a specific use-case. In our case, we want to

be able to manage the objects of our project:

  

- Create a new object (ex: a new User or a new Place)

- Retrieve an object from a file, a database etc…

- Do operations on objects (count, compute stats, etc…)

- Update attributes of an object

- Destroy an object

  

### Learning Objectives

  

## General

 - How to create a Python package
   
  - How to create a command interpreter in Python using the cmd module
   
   - What is Unit testing and how to implement it in a large project
   
   - How to serialize and deserialize a Class
   
   - How to write and read a JSON file
   
   - How to manage datetime
   
   - What is an UUID
   
   - What is *args and how to use it
   
   - What is **kwargs and how to use it
   
   - How to handle named arguments in a function

  
  

## Execution

  
Your shell should work like this in interactive mode:

  
```
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF help quit

(hbnb)
(hbnb)
(hbnb) quit
$
```

But also in non-interactive mode: (like the Shell project in C)

```
$ echo "help" | ./console.py

(hbnb)

Documented commands (type help <topic>):
========================================

EOF help quit
(hbnb)
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

  
Documented commands (type help <topic>):
========================================
EOF help quit
(hbnb)
$

```

## Usage Examples

**Launching the console**
```
$ ./console.py
(hbnb) 
```
**Creating a new object**
```
(hbnb) create
** class name missing **
(hbnb) create User
670265eb-5982-489e-8b92-2dff054f0776
```
**Show an object**
```
(hbnb) show User
** instance id missing **
(hbnb) show User 670265eb-5982-489e-8b92-2dff054f0776
[User] (670265eb-5982-489e-8b92-2dff054f0776) {'created_at': datetime.datetime(2020, 2, 19, 18, 8, 58, 458246), 'id': '670265eb-5982-489e-8b92-2dff054f0776', 'updated_at': datetime.datetime(2020, 2, 19, 18, 8, 58, 458261)}
```
**Update an object**
```
(hbnb) all
["[User] (70f71c16-962b-48ad-9df8-9203fe23d612) {'created_at': datetime.datetime(2020, 2, 19, 18, 11, 32, 341144), 'id': '70f71c16-962b-48ad-9df8-9203fe23d612', 'updated_at': datetime.datetime(2020, 2, 19, 18, 11, 32, 341161)}"]
(hbnb) update
** class name missing **
(hbnb) update User
** instance id missing **
(hbnb) update User 70f71c16-962b-48ad-9df8-9203fe23d612
** attribute name missing **
(hbnb) update User 70f71c16-962b-48ad-9df8-9203fe23d612  Age "20"
(hbnb) all
["[User] (70f71c16-962b-48ad-9df8-9203fe23d612) {'Age': 20, 'created_at': datetime.datetime(2020, 2, 19, 18, 11, 32, 341144), 'id': '70f71c16-962b-48ad-9df8-9203fe23d612', 'updated_at': datetime.datetime(2020, 2, 19, 18, 13, 9, 937933)}"]
(hbnb)
```
**Destroy an object**
```
(hbnb) destroy
** class name missing **
(hbnb) destroy User
** instance id missing **
(hbnb) destroy User 670265eb-5982-489e-8b92-2dff054f0776
(hbnb)
```
