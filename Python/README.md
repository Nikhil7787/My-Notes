# Python

## ✅ Basic Syntax and Data Types

### ▶ Variables 

Definition:- A variable in Python is a named location used to store data in the computer's memory. It acts as a placeholder for values that can be manipulated or referenced in a program.

Rules for Naming Variables:-

1.	Variable names can contain letters (a-z, A-Z), digits (0-9), and underscores (_). </br>
2.	Variable names must start with a letter or an underscore.  </br>
3.	Variable names are case-sensitive (myVar, MyVar, and myvar are different variables).  </br>
4.	Python keywords cannot be used as variable names. </br>
5.	Variable names should be descriptive and meaningful to improve code readability.  </br>

Variable Assignment:- To assign a value to a variable, you use the assignment operator =. The value on the right side of the = is assigned to the variable on the left side.

```
# Variable assignment
x = 10
name = "John"
is_student = True

```
Variable Reassignment:- You can change the value of a variable by assigning a new value to it. </br>
```
x = 10
print(x)   # Output: 10

x = 20
print(x)   # Output: 20
```
Variable Scope:-
Variables can have different scopes, such as global and local. A variable declared outside of any function or block has a global scope, while a variable declared within a function has a local scope.

```
# Global variable
x = 10

def my_function():
    # Local variable
    y = 20
    print("Local variable y:", y)

my_function()
print("Global variable x:", x)
```

Constants:- Although Python doesn't have built-in support for constants, variables that are intended to be constant are typically named in all capital letters to indicate their immutability.
```
PI = 3.14
GRAVITY = 9.8
```
Summary:-
1.	Variables are named locations used to store data in memory.
2.	Python variables don't have a fixed data type and can hold different types of data.
3.	Variable names must follow certain rules and conventions.
4.	You can print variables using the print() function.
5.	Variable values can be reassigned.
6.	Variables can have different scopes, such as global and local.
7.	Constants are typically represented using all capital letters.


### ▶ data types

Definition: - In Python, data types represent the type or kind of data that a variable can store. Python supports various built-in data types to handle different kinds of data. </br>

Common Data Types: - </br>
1.	Numeric Types: </br>
•	int: Represents integer values. </br>
•	float: Represents floating-point (decimal) values. </br>
•	complex: Represents complex numbers with real and imaginary parts. </br>
2.	Sequence Types:  </br>
•	str: Represents strings, which are sequences of characters. </br> 
•	list: Represents lists, which are ordered collections of items. </br>
•	tuple: Represents tuples, which are ordered and immutable collections of items. </br>
3.	Boolean Type: </br>
•	bool: Represents boolean values (True or False). </br>
4.	Mapping Type: </br>
•	dict: Represents dictionaries, which are unordered collections of key-value pairs. </br>
5.	Set Types: </br> 
•	set: Represents unordered collections of unique items. </br>
•	frozenset: Represents immutable sets. </br>

Checking Data Types:-
You can use the type() function to determine the data type of a variable or value.
```
# Checking data types
x = 10
print(type(x))   # Output: <class 'int'>

y = 3.14
print(type(y))   # Output: <class 'float'>

name = "Alice"
print(type(name))   # Output: <class 'str'>

is_student = True
print(type(is_student))   # Output: <class 'bool'>

```

Type Conversion (Casting):-
Python allows you to convert data from one type to another using type conversion functions like int(), float(), str(), list(), tuple(), dict(), etc.
```
# Type conversion
x = 10
y = float(x)   # Convert integer to float
print(y)       # Output: 10.0

z = str(x)     # Convert integer to string
print(z)       # Output: '10'

```
Immutable vs. Mutable Data Types:- </br>
Immutable: Data types like int, float, str, tuple, and frozenset are immutable, meaning their values cannot be changed after creation. </br>
Mutable: Data types like list, dict, set, and bytearray are mutable, meaning their values can be changed after creation. </br>

Summary:- <br/>
 1.	Python supports various built-in data types to handle different kinds of data. <br/>
2.	Common data types include numeric types, sequence types, boolean type, mapping type, and set types. <br/>
3.	You can use the type() function to check the data type of a variable or value. <br/> 
4.	Type conversion functions allow you to convert data from one type to another. <br/>
5.	Immutable data types cannot be changed after creation, while mutable data types can be modified.

 

### ▶ arithmetic operations

Definition:-
Arithmetic operations in Python are used to perform mathematical calculations on numeric data types such as integers and floats. Python supports standard arithmetic operators for addition, subtraction, multiplication, division, exponentiation, and modulus. </br> 
</br>
Arithmetic Operators:-</br>
1.	Addition (+): Adds two operands. </br>
2.	Subtraction (-): Subtracts the second operand from the first. </br>
3.	Multiplication (*): Multiplies two operands. </br>
4.	Division (/): Divides the first operand by the second (returns a float). </br>
5.	Floor Division (//): Divides the first operand by the second and rounds down to the nearest integer. </br> 
6.	Exponentiation (**): Raises the first operand to the power of the second. </br>
7.	Modulus (%): Returns the remainder of the division of the first operand by the second.</br>


```
# Addition
result_addition = 10 + 5
print("Addition:", result_addition)   # Output: 15

# Subtraction
result_subtraction = 20 - 8
print("Subtraction:", result_subtraction)   # Output: 12

# Multiplication
result_multiplication = 6 * 4
print("Multiplication:", result_multiplication)   # Output: 24

# Division
result_division = 20 / 3
print("Division:", result_division)   # Output: 6.666666666666667

# Floor Division
result_floor_division = 20 // 3
print("Floor Division:", result_floor_division)   # Output: 6

# Exponentiation
result_exponentiation = 2 ** 3
print("Exponentiation:", result_exponentiation)   # Output: 8

# Modulus
result_modulus = 20 % 3
print("Modulus:", result_modulus)   # Output: 2

```
Assignment Operators with Arithmetic Operations:-
Python provides shorthand assignment operators to perform arithmetic operations and assign the result back to the variable. </br>

```
x = 10
x += 5   # Equivalent to: x = x + 5
print(x)   # Output: 15

y = 20
y -= 8   # Equivalent to: y = y - 8
print(y)   # Output: 12

z = 6
z *= 4   # Equivalent to: z = z * 4
print(z)   # Output: 24

```

Summary:- <br/>
1.	Python supports standard arithmetic operators for addition, subtraction, multiplication, division, exponentiation, floor division, and modulus. </br>
2.	Order of operations (precedence) follows the standard rules (PEMDAS/BODMAS). </br>
3.	Shorthand assignment operators can be used to perform arithmetic operations and assign the result back to the variable. </br>


### ▶ String Manipulation

Definition:- 
String manipulation refers to the process of modifying, joining, splitting, searching, and formatting strings in Python. Strings are sequences of characters, and Python provides various built-in methods and operators for working with strings efficiently. </br>

Basic String Operations:- </br>
1.	Concatenation: Combining two or more strings into one. </br>
2.	Repetition: Repeating a string multiple time. </br>
3.	Indexing: Accessing individual characters in a string using index positions. </br>
4.	Slicing: Extracting a substring from a string using a range of indices. </br>
5.	Length: Finding the length of a string using the len() function. </br>
6.	Membership: Checking if a substring exists within a string using the in keyword. </br>


```
# Concatenation
str1 = "Hello"
str2 = "World"
result_concatenation = str1 + " " + str2
print("Concatenation:", result_concatenation)   # Output: Hello World

# Repetition
str_repeated = "abc" * 3
print("Repetition:", str_repeated)   # Output: abcabcabc

# Indexing
my_string = "Python"
print("Character at index 0:", my_string[0])   # Output: P
print("Character at index 3:", my_string[3])   # Output: h

# Slicing
substring = my_string[1:4]
print("Substring:", substring)   # Output: yth

# Length
length = len(my_string)
print("Length of string:", length)   # Output: 6

# Membership
contains_python = "Python" in my_string
print("Contains 'Python'?", contains_python)   # Output: True

```

Common String Methods:- </br>
1.	upper(): Converts all characters in a string to uppercase.  </br>
2.	lower(): Converts all characters in a string to lowercase.  </br> 
3.	capitalize(): Capitalizes the first character of a string. </br> 
4.	title(): Capitalizes the first character of each word in a string. </br> 
5.	strip(): Removes leading and trailing whitespace from a string. </br> 
6.	replace(old, new): Replaces occurrences of a substring with another substring. </br> 
7.	split(separator): Splits a string into a list of substrings based on a separator. </br> 
8.	join(iterable): Joins elements of an iterable (e.g., list) into a single string using the specified separator.

```
my_string = "    hello world    "

# Upper and Lower
print("Uppercase:", my_string.upper())   # Output: HELLO WORLD
print("Lowercase:", my_string.lower())   # Output: hello world

# Capitalize and Title
print("Capitalized:", my_string.capitalize())   # Output: Hello world
print("Title:", my_string.title())   # Output: Hello World

# Strip
print("Stripped:", my_string.strip())   # Output: hello world

# Replace
print("Replaced:", my_string.replace("world", "universe"))   # Output: hello universe

# Split and Join
words = my_string.strip().split()
print("Split:", words)   # Output: ['hello', 'world']
joined_string = "-".join(words)
print("Joined:", joined_string)   # Output: hello-world

```
String Formatting:- </br>
String formatting allows you to create formatted strings with placeholders for variable values. </br>

Old Style Formatting using % operator. </br>
New Style Formatting using format() method. </br>
Formatted String Literals (f-strings) introduced in Python 3.6. </br>

```
# Old Style Formatting
name = "Alice"
age = 30
formatted_string = "Name: %s, Age: %d" % (name, age)
print("Old Style Formatting:", formatted_string)   # Output: Name: Alice, Age: 30

# New Style Formatting
formatted_string = "Name: {}, Age: {}".format(name, age)
print("New Style Formatting:", formatted_string)   # Output: Name: Alice, Age: 30

# Formatted String Literals (f-strings)
formatted_string = f"Name: {name}, Age: {age}"
print("f-strings:", formatted_string)   # Output: Name: Alice, Age: 30

```
Summary:-

1.	String manipulation involves modifying, joining, splitting, searching, and formatting strings.
2.	Basic string operations include concatenation, repetition, indexing, slicing, length calculation, and membership testing.
3.	Python provides numerous string methods for common string manipulations.
4.	String formatting allows you to create formatted strings with placeholders for variable values.







### ▶ Lists 
### ▶ tuples
### ▶ Dictionaries

## ✅ Control Flow

### ▶ Conditional statements (if, elif, else)
### ▶ Loops (for loops, while loops)
### ▶ Loop control statements (break, continue)

## ✅ Functions

### ▶ Defining functions
### ▶ Passing arguments to functions
### ▶ Returning values from functions
### ▶ Scope of variables (local vs global)
### ▶ Modules and Packages

## ✅  File Handling

### ▶ Reading from and writing to files
### ▶ Working with different file formats (text files, CSV, JSON)

## ✅ Error Handling
 
### ▶ Exception handling with try-except blocks
### ▶ Raising exceptions

## ✅ Object-Oriented Programming (OOP)

### ▶ Introduction to classes and objects
### ▶ Inheritance
### ▶ Encapsulation
### ▶ Polymorphism

## ✅ Data Structures and Algorithms

### ▶ Understanding complex data structures (sets, dictionaries, stacks, queues)
### ▶ Implementing basic algorithms (sorting, searching)

## ✅ Advanced Topics

### ▶ Lambda Functions

### ▶ Functional Programming Tools
map Function: Explain how map applies a function to all items in an input list and returns a new list with the results. </br>
filter Function: Teach filter for selecting elements from an iterable based on a function condition. </br>
reduce Function: Introduce reduce from the functools module for applying a function to the elements of an iterable to reduce them to a single value. 

### ▶ Decorators
### ▶ Generators
### ▶ Context Managers

## ✅ Concurrency and Parallelism

### ▶ Threading 
### ▶ Multiprocessing
### ▶ Asynchronous programming with async/await


