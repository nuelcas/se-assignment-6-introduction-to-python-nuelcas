[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15307145&assignment_repo_type=AssignmentRepo)

# SE-Assignment-6

Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

Questions:

1. Python Basics:

   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.

   Answer:
   Python is a programming language that is easy to learn and use. It was created in the late 1980s by Guido van Rossum and has become one of the most popular languages today. Python is like a tool that helps you write instructions for a computer to follow. It's known for being simple and clear, making it a great choice for beginners and experts alike.
   Some of key features of Python are: readable and simple syntax, large community and libraries, works on different OS like Windows, macOS, Linux, its versatility makes it easy to be used in different projects.
   Python is used for Web Development, Data Science and Analysis, Artificial Intelligence (AI) and Machine Learning, Automation.

2. Installing Python:

   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.

   Answer:
   Steps to install Python on Windows"

   1. Go to the official Python website(https://www.python.org/downloads/) and download Python installer.
   2. Run the Installer by opening the downloaded python-XXX.exe file. Check "Add Python to PATH" and click "Install Now".

   How to verify the Python installation:
   Open Command Prompt, type cmd on the search icon of your PC, press Enter, type "python --version" to check the installed version.

   How to set up a virtual environment for Django Project using Git Bash:

   1. Open Git Bash and run: "pip install virtualenv"
   2. Navigate to your project folder by running: "cd path/to/your/project" (since i stored my project on C drive, I will run: "cd c:/")
   3. Run: "virtualenv venv" to create virtual environment for your project. Note: "venv" is the name for your virtual environment, you can change it to any name of your choice.
   4. Run: "source venv/Scripts/activate" to activate virtual environment.
   5. Run: "pip install django" to install Django.
   6. Run: "django-admin startproject myproject" to create Django project. Note: "myproject" is your project name.

3. Python Syntax and Semantics:

   - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

   Answer:
   Simple Python program: print("Hello, World!")

   Explanation of the basic syntax elements:
   `print`: This is a function that tells the computer to display something on the screen.
   `("Hello, World!")`: This is the argument for the print function, enclosed in parentheses. It's a string (a sequence of characters) that you want to display.
   `(" ")`: Quotation marks are used to indicate the beginning and end of a string

4. Data Types and Variables:

   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.

   Answers:

   Basic Data Types in Python

   1. Integer (int): Whole numbers, like 5 or -3.
   2. Float (float): Decimal numbers, like 3.14 or -0.001.
   3. String (str): Text, enclosed in quotes, like "hello" or 'world'.
   4. Boolean (bool): True or False values.
   5. List (list): Ordered collection of items, like [1, 2, 3] or ["apple", "banana"].
   6. Dictionary (dict): Key-value pairs, like {"name": "John", "age": 17}.

   How to create and use variables of different data types:

   # Creating variables of different data types

   age = 17 # Integer
   height = 5.9 # Float
   name = "Alex" # String
   is_student = True # Boolean
   favorite_numbers = [3, 7, 21] # List
   student_info = {"name": "Alex", "age": 17, "grade": "A"} # Dictionary

   # Using the variables

   print(f"Name: {name}")
   print(f"Age: {age}")
   print(f"Height: {height} feet")
   print(f"Is student: {is_student}")
   print(f"Favorite numbers: {favorite_numbers}")
   print(f"Student info: {student_info}")

5. Control Structures:

   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.

   Answers:

   `if-else` statement: It's like making a choice. If something is true, you do one thing; if it's not true, you do something else.

   Example:

   age = 17

   if age >= 18:
   print("You can vote!")
   else:
   print("You cannot vote yet.")

   In the above example, Python checks if age is 18 or older. If it is, it prints "You can vote!". If age is less than 18, it prints "You cannot vote yet."

   `for loop`:It's like doing something over and over again.

   Example:

   fruits = ["apple", "banana", "cherry"]

   for fruit in fruits:
   print(fruit)

   In this example, the `for loop` goes through each item in the fruits list ("apple", "banana", "cherry") and prints each item one by one.

6. Functions in Python:

   - What are functions in Python, and why are they useful? Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.

   Answer:

   Functions in Python are like recipes. They are blocks of code that you can use over and over again to perform a specific task. They're useful because they help you write cleaner code, avoid repeating yourself, and organize your program better.

   Python Function:

   def add_numbers(a, b):
   sum = a + b
   return sum

   To use the above function, you call it with two numbers as arguments:

   result = add_numbers(3, 5)
   print(result) # Output: 8

7. Lists and Dictionaries:

   - Describe the differences between lists and dictionaries in Python. Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.

   Answer:

   Lists in Python are like arrays that store ordered collections of items, like numbers or words. Dictionaries, on the other hand, store data as key-value pairs where each piece of data is accessed by its key rather than its position. Lists are ordered collections of items that can be accessed and manipulated using their positions (indices).
   Dictionaries are unordered collections of items where each item is accessed using a key.

   A simple script to show the differences:

   # Creating a list of numbers

   numbers = [1, 2, 3, 4, 5]

   # Creating a dictionary with key-value pairs

   person = {
   "name": "Alice",
   "age": 25,
   "city": "New York"
   }

   # Accessing elements in a list

   print(numbers[0]) # Prints: 1

   # Accessing elements in a dictionary

   print(person["name"]) # Prints: Alice

   # Adding elements to a list

   numbers.append(6)
   print(numbers) # Prints: [1, 2, 3, 4, 5, 6]

   # Adding elements to a dictionary

   person["job"] = "Engineer"
   print(person) # Prints: {'name': 'Alice', 'age': 25, 'city': 'New York', 'job': 'Engineer'}

   # Updating elements in a list

   numbers[0] = 10
   print(numbers) # Prints: [10, 2, 3, 4, 5, 6]

   # Updating elements in a dictionary

   person["age"] = 26
   print(person) # Prints: {'name': 'Alice', 'age': 26, 'city': 'New York', 'job': 'Engineer'}

   # Removing elements from a list

   numbers.remove(3)
   print(numbers) # Prints: [10, 2, 4, 5, 6]

   # Removing elements from a dictionary

   del person["city"]
   print(person) # Prints: {'name': 'Alice', 'age': 26, 'job': 'Engineer'}

8. Exception Handling:

   - What is exception handling in Python? Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python script.

   Answer:

   Exception handling in Python is a way to manage errors that can happen when a program runs. Here is a quick breakdown:

   `Try block`: You put the code that might have an error inside this block.

   `Except block`: You write code here that runs if there's an error in the try block. It helps you handle the error gracefully.

   `Finally block`: You can put code here that always runs, no matter if there was an error or not in the try block. It's used for cleanup tasks.

   Example:

   try:
   x = int(input("Enter a number: "))
   y = 10 / x # This might cause an error if x is 0
   print("y =", y)
   except ZeroDivisionError:
   print("Cannot divide by zero!")
   finally:
   print("This always executes, no matter what.")

9. Modules and Packages:

   - Explain the concepts of modules and packages in Python. How can you import and use a module in your script? Provide an example using the `math` module.

   Answer:

   Module: A file containing Python code. It can define functions, variables, and classes that you can use in other Python files.

   Package: A collection of modules grouped together. Packages are used to organize and distribute Python code.

   To use a module in your script:

   Importing: Use the `import` keyword followed by the module name.

   Using module: You can then use functions, variables, or classes from the module by prefixing them with the module name.

   Example using the math module:

   # Importing the math module

   import math

   # Using functions from the math module

   print(math.sqrt(25)) # Outputs: 5.0 (square root of 25)
   print(math.pi) # Outputs: 3.141592653589793 (value of pi)

10. File I/O:

    - How do you read from and write to files in Python? Write a script that reads the content of a file and prints it to the console, and another script that writes a list of strings to a file.

    Answer:

    Script to read from a file and print its content:

    # Open the file in read mode ('r')

    with open('filename.txt', 'r') as file:

    # Read the entire content of the file

    content = file.read()

    # Print the content to the console

    print(content)

    Script to write a list of strings to a file:

    # Example list of strings

    my_list = ["Hello", "Python", "World"]

    # Open the file in write mode ('w')

    with open('output.txt', 'w') as file:

    # Write each string from the list to the file

    for string in my_list:
    file.write(string + "\n")

Explanation:

Reading a file (open('filename.txt', 'r')): Use open() function with 'r' to open a file in read mode.

file.read() reads the entire content of the file into a string variable (content).

Use print(content) to display the content in the console.

Writing to a file (open('output.txt', 'w')): Use open() function with 'w' to open a file in write mode.

Loop through each item in my_list and use file.write(string + "\n") to write each string to the file, with a newline character \n to separate them.

These scripts show the basics of how to handle files in Python. Remember to replace 'filename.txt' and 'output.txt' with your actual file names.

# Submission Guidelines:

- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.
- Submit your completed assignment by [due date].
