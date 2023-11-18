# Python_demo_code01
just py code with comments
This will help a beiginner to have breif idea about python and its commands.


reference : www.w3schools.com

# Python Basics Cheatsheet

A quick reference guide for Python basics.

## Table of Contents

1. [Variables and Data Types](#variables-and-data-types)
2. [Control Structures](#control-structures)
3. [Functions](#functions)
4. [Lists](#lists)
5. [Dictionaries](#dictionaries)
6. [Loops](#loops)
7. [File Handling](#file-handling)

## Variables and Data Types

### Variables
```python
# Variables
x = 5
y = 'Hello'
z = 3.14

# Data Types
int_variable = 10
str_variable = 'Python'
float_variable = 3.14
bool_variable = True

# If-Else Statements
x = 10
if x > 5:
    print('x is greater than 5')
else:
    print('x is less than or equal to 5')

# For Loop
for i in range(5):
    print(i)

# While Loop
count = 0
while count < 5:
    print(count)
    count += 1

# Defining a Function
def greet(name):
    return f'Hello, {name}!'

print(greet('Alice'))

# Creating Lists
my_list = [1, 2, 3, 4, 5]

# List Operations
my_list.append(6)
my_list.remove(3)
print(my_list)

# Creating Dictionaries
my_dict = {'name': 'Alice', 'age': 30, 'city': 'New York'}

# Dictionary Operations
print(my_dict['name'])
my_dict['age'] = 31
print(my_dict)

# Reading from a File
with open('file.txt', 'r') as file:
    data = file.read()
    print(data)

# Writing to a File
with open('file.txt', 'w') as file:
    file.write('Hello, Python!')


This is a basic structure that you can expand upon by adding more Python concepts, examples, and explanations to create a comprehensive cheatsheet. You can paste this into a Markdown file (e.g., `python_cheatsheet.md`) in your GitHub repository and customize it further according to your preferences or the specific topics you want to cover.
