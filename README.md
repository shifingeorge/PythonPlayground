# Python Programming Roadmap & Cheat Sheet

This markdown file serves as a guide and quick reference to Python's language syntax, key features, and functionalities. 

# Table of Contents

 1. [Introduction to Python](#introduction-to-python)
 2. [Variables and Data Types](#variables-and-data-types)
 3. [Control Flow](#control-flow)
 4. [Functions](#functions)
 5. [Classes (Object-oriented programming)](#classes-object-oriented-programming)
 6. [Error Handling](#error-handling)
 7. [File Input/Output](#file-inputoutput)
 8. [Python Libraries](#python-libraries)
 9. [Tips & Tricks](#tips--tricks)
 10. [Resources for Further Learning](#resources-for-further-learning)


## Introduction to Python

Python is an interpreted, high-level general-purpose programming language. Its design philosophy emphasizes code readability with its use of significant indentation. 

```python
print("Hello, World!")
```

## Variables and Data Types

In Python, variables are containers for storing data values. Python has the following data types built-in by default, in these categories:

- **Text Type**: _`str`_
- **Numeric Types**: _`int`, `float`, `complex`_
- **Sequence Types**: _`list`, `tuple`, `range`_
- **Mapping Type**: _`dict`_
- **Set Types**: _`set`, `frozenset`_
- **Boolean Type**: _`bool`_
- **Binary Types**: _`bytes`, `bytearray`, `memoryview`_

```python
x = "Hello World" #str	
x = 20 #int	
x = 20.5 #float	
x = 1j #complex	
x = ["apple", "banana", "cherry"] #list	
x = ("apple", "banana", "cherry") #tuple	
x = range(6) #range	
x = {"name" : "John", "age" : 36} #dict	
x = {"apple", "banana", "cherry"} #set	
x = frozenset({"apple", "banana", "cherry"}) #frozenset	
x = True #bool	
x = b"Hello" #bytes	
x = bytearray(5) #bytearray	
x = memoryview(bytes(5)) #memoryview
```

## Control Flow

Control flow is the order in which individual statements, instructions or function calls of an imperative program are executed or evaluated.

- if ... Else
  ```python
  a = 33
  b = 200
  if b > a:
    print("b is greater than a")
  ```
- while Loops
  ```python
  i = 1
  while i < 6:
    print(i)
    i += 1
  ```
- For Loops
  ```python
  fruits = ["apple", "banana", "cherry"]
  for x in fruits:
    print(x)
  ```

## Functions

A function is a block of code which only runs when it is called. You can pass data, known as parameters, into a function. A function can return data as a result.

```python
def my_function():
  print("Hello from a function")
my_function()
```

## Classes (Object-oriented programming)

Python is an object oriented programming language. Almost everything in Python is an object, with its properties and methods. A Class is like an object constructor, or a "blueprint" for creating objects.

```python
class MyClass:
  x = 5
p1 = MyClass()
print(p1.x)
```

## Error Handling

Python has several built-in exceptions that force your program to output an error when something in the program goes wrong.

- Raising an Exception
  ```python
  x = -1
  if x < 0:
    raise Exception("Sorry, no numbers below zero")
  ```
- The try ... except Block
  ```python
  try:
  print(variable)
  except:
    print("An exception occurred")
  ```
## File Input/Output

Python allows you to work with files (read and write files).

- Writing to a File
  ```python
  f = open("demofile.txt", "w")
  f.write("Now the file has content!")
  f.close()
  ```
- Reading a File
  ```python
  f = open("demofile.txt", "r")
  print(f.read())
  f.close()
  ```
## Python Libraries

Python has a rich collection of libraries. These are some of them:

1. NumPy
2. SciPy
3. Matplotlib
4. Pandas

## Tips & Tricks

Python is filled with subtle coding techniques that can make your code more efficient and easier to understand. Here are a few:

### List Comprehensions

List comprehensions offer a concise way to create lists based on existing lists. Here is an example:
```python
# Traditional method
numbers = [1, 2, 3, 4, 5]
squares = []
for n in numbers:
  squares.append(n**2)

# Using List Comprehensions
squares = [n**2 for n in numbers]
```

### Use of `enumerate()`

When you need to iterate over a list and use both its elements and their indexes, `enumerate()` becomes invaluable. It allows us to loop over something and have an automatic counter.
```python
list = ["apple", "banana", "mango"]
for i, item in enumerate(list):
    print(f"Item {i} is {item}")
```

### One-Liners for Conditional Assignment

Python allows a single line of code to assign a value to a variable based on a condition.
```python
condition = True
x = 1 if condition else 0  # If condition is True, x is 1. Else, x is 0
```

## Resources for Further Learning

Here are some resources to further enhance your Python knowledge and skills:

#### 1. Python's Official Documentation: https://docs.python.org/3/
#### 2. Real Python: https://realpython.com/
#### 3. Codecademy's Python Course: https://www.codecademy.com/learn/learn-python-3
#### 4. r/Python Subreddit: https://www.reddit.com/r/Python/

## Contributions Welcome 🌟

If you've discovered new resources, tips, or information that could benefit Python enthusiasts in their learning journey, feel free to contribute to this Markdown file!

### How to Contribute

1. Fork this repository.
2. Make your changes or additions to the Markdown file.
3. Create a pull request describing your changes and their purpose.
4. Your contribution will be reviewed and merged to help Python enthusiasts!

Let's make this resource better together! 🐍💻
