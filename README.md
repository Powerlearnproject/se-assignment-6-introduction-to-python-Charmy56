[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/WfNmjXUk)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15318095&assignment_repo_type=AssignmentRepo)
# SE-Assignment-6
 Assignment: Introduction to Python
Instructions:
Answer the following questions based on your understanding of Python programming. Provide detailed explanations and examples where appropriate.

 Questions:

1. Python Basics:
   - What is Python, and what are some of its key features that make it popular among developers? Provide examples of use cases where Python is particularly effective.
    - Python is a high-level, interpreted programming language known for its easy-to-read syntax and versatility. Key features include:

     a. Simplicity: Python’s syntax is clear and intuitive, making it an excellent language for beginners.
     b. Versatility: It can be used for web development, data analysis, artificial intelligence, scientific computing, and more.
     c. Extensive Libraries: Python has a vast standard library and many third-party libraries for various tasks.
Python is particularly effective in:

    a. Data Analysis & Machine Learning: With libraries like Pandas and Scikit-learn, Python is great for crunching numbers and building ML models.
    b. Web Development: Frameworks like Django and Flask make web application development quick and efficient.
    c. Automation: Python scripts can automate mundane tasks, from file organization to network configuration.
    d. Scientific Computing: Libraries like NumPy and SciPy are used extensively in scientific research for complex computations.

2. Installing Python:
   - Describe the steps to install Python on your operating system (Windows, macOS, or Linux). Include how to verify the installation and set up a virtual environment.
   I will describe how to do the installation on windows.
   a. Download Python by
Visiting the Python Releases for Windows page on the official Python website.
Choose the latest stable release (currently Python 3.12.4) that matches your system architecture (64-bit or ARM64).
Download the Windows installer (64-bit) or Windows installer (ARM64) based on your system.
b. Run the Installer
 by double-clicking the downloaded installer file to launch the setup wizard.
In the setup window, check the box that says “Add Python 3.12 to PATH.” This ensures that Python is added to your system’s environment variables.
Click the “Install Now” button to begin the installation. It will take a few minutes to complete.
c. Verify the Installation by
Openning the Command Prompt (search for “cmd” in the Start menu).
Type python --version and press Enter. You should see the installed Python version (e.g., “Python 3.12.4”).
d. Set Up a Virtual Environment (Optional):
To manage Python packages and dependencies, it’s recommended to create a virtual environment.
Open the Command Prompt and navigate to the directory where you want to create your project.
e. Run the following commands:
python -m venv myenv
source myenv\Scripts\activate
Replace “myenv” with your preferred environment name.
Your virtual environment is now active. You can install packages using pip.

3. Python Syntax and Semantics:
 - Write a simple Python program that prints "Hello, World!" to the console. Explain the basic syntax elements used in the program.

      print("Hello, World!")

4. Data Types and Variables:
   - List and describe the basic data types in Python. Write a short script that demonstrates how to create and use variables of different data types.
Integer (int): Used for whole numbers e.g., 5, -10, 0.
Floating-Point (float): Represents decimal numbers (e.g., 3.14, -2.5).
String (str): Stores sequences of characters (e.g., “Hello, World!”).
Boolean (bool): Represents truth values (True or False).
demonstrating how to create variables of different data types:

Integer
first_integer = 20
print("Integer value:", first_integer)

Floating-Point
first_float = 2.15
print("Float value:", first_float)

 String
first_string = "Hello, World!"
print("String value:", first_string)

Boolean
first_boolean = True
print("Boolean value:", first_boolean)

5. Control Structures:
   - Explain the use of conditional statements and loops in Python. Provide examples of an `if-else` statement and a `for` loop.
     Conditional statements programmers   to make decisions based on conditions. They control the flow of the program.
     # if-else-example
     result = "Pass" if score >= 55 else "Fail"
     # for-loop-example
     for i in range(3):
    print(i)
Output: 0 1 2 

6. Functions in Python:
   - What are functions in Python, and why are they useful? 
      Functions in Python are blocks of reusable code that perform specific tasks. They allow programmers to break down complex problems into smaller, manageable parts. They are useful because:
      a. Modularity: Functions help organize code by dividing it into logical units. You can create separate functions for different tasks, making your program more readable and maintainable.
      b. Reusability: Once defined, functions can be called multiple times from different parts of your program. This reusability reduces redundancy and promotes efficient coding.
      c. Abstraction: Functions abstract away implementation details. You can use a function without knowing how it works internally, focusing on what it accomplishes.
   Write a Python function that takes two arguments and returns their sum. Include an example of how to call this function.
def add_numbers(num1, num2):
    return num1 + num2

# Calling the function
result = add_numbers(2, 6)
print("Sum:", result)

7. Lists and Dictionaries:
   - Describe the differences between lists and dictionaries in Python.
   Lists are ordered collections of elements, similar to arrays in other languages. On the other hand, dictionaries store data as key-value pairs (unodered) 
   Lists are best for sequential data, while dictionaries are optimized for data retrieval by specific identifiers.

    Write a script that creates a list of numbers and a dictionary with some key-value pairs, then demonstrates basic operations on both.
     # Create a list of numbers
my_list = [1, 2, 3, 4, 5]

dictionary with key-value pairs
my_dict = {
    'orange': 'red',
    'pineapple': 'yellow',
    'guava': 'pink'
}

 Accessing elements:
print("List element at index 2:", my_list[2])  # Output: 3
print("Color of pineapple:", my_dict['pineapple'])  # Output: yellow

 Adding an entry to the dictionary:
my_dict['grape'] = 'grape'

Changing an entry:
my_list[3] = 10

Deleting an entry:
del my_dict['grape']
Looping over keys in the dictionary:
for fruit in my_dict:
    print(f"Fruit: {fruit}, Color: {my_dict[fruit]}")

Getting the length of the list:
list_length = len(my_list)
print("List length:", list_length)

Checking if a key exists in the dictionary:
if 'guava' in my_dict:
    print("guava exists in the dictionary")

 Sorting the dictionary by keys:
sorted_dict = {k: my_dict[k] for k in sorted(my_dict)}

Displaying the sorted dictionary:
print("Sorted dictionary:", sorted_dict)

8. Exception Handling:
   - What is exception handling in Python?
   Exception handling in Python allows you to gracefully handle unexpected errors during program execution. It prevents your program from crashing and provides a way to recover or take alternative actions when errors occur.
    Provide an example of how to use `try`, `except`, and `finally` blocks to handle errors in a Python scrip
   
The try block contains the code that might raise an exception.
The except block handles specific exceptions that occur within the try block.
The finally block always executes, whether an exception occurs or not.
example:
def divide(a, b):
    try:
        result = a / b
        print("Result:", result)
    except ZeroDivisionError:
        print("Error: You cannot divide by zero.")
    finally:
        print("Cleanup: Always executed (even if an exception occurs).")

Example-application
divide(14, 2)  # Output: Result: 7.0, Cleanup: Always executed
divide(14, 0)  # Output: Error: You cannot divide by zero., Cleanup: Always executed

9. Modules and Packages:
   - Explain the concepts of modules and packages in Python.
   A module is a single file containing Python code. It can include functions, variables, and classes. On the other hand, a package is a collection of related modules organized in a directory hierarchy. They help in managing large projects by grouping related functionality together.

    How can you import and use a module in your script? 
   To import a module, use the import statement followed by the module name (e.g., import math).
   Provide an example using the `math` module.
   import math
result = math.sq(10)
print("Square  of 10:", result)  # Output: 100.0

10. File I/O:
    - How do you read from and write to files in Python? 
     To read from a file,  use the open() function to open the file in read mode ("r"). Then use methods like read(), readline(), or readlines() to retrieve the file content.
     To write to a file, open it in write mode ("w"). If the file doesn’t exist, Python will create it.
     Then use the write() method to add content to the file.
    Write a script that reads the content of a file and prints it to the console, 

file_path = 'sample.txt'
try:
    with open(file_path, 'r') as file:
        file_content = file.read()
        print("File Content:\n", file_content) 
except FileNotFoundError:
    print(f"File '{file_path}' not found.")
except Exception as e:
    print(f"An error occurred: {e}")

 REFERENCES
 used W3school for my answers - *python tutorial- *python intro*
# Submission Guidelines:
- Your answers should be well-structured, concise, and to the point.
- Provide code snippets or complete scripts where applicable.
- Cite any references or sources you use in your answers.



