---
title: "Lecture4 # Variables and Comments in Python"
datePublished: Tue Oct 10 2023 14:09:15 GMT+0000 (Coordinated Universal Time)
cuid: clnkeeirt00000ajmcuz51b4l
slug: lecture4-variables-and-comments-in-python
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1696946912825/88b29b4a-529d-46e0-a382-60fcbd9f4724.png
tags: python, devops, python-beginner, devops-articles, masterwithhamza

---

Variables and comments are essential elements in Python programming that help you manage and document your code effectively. Let's explore them in detail:

**My Python codes:** [https://masterwithhamza@bitbucket.org/hamxaflutterapps/mypythoncodes.git](https://masterwithhamza@bitbucket.org/hamxaflutterapps/mypythoncodes.git)

## **Variables in Python**

In Python, variables are used to store and manage data. You can think of a variable as a named container that holds a value. Here's how you declare and use variables in Python:

### **Variable Declaration**

To declare a variable, you simply choose a name for it and assign a value using the assignment operator `=`. You don't need to explicitly specify the data type; Python infers it automatically.

```python
# Variable assignment
age = 30
name = "Hamza"
pi = 3.14
is_student = True
```

### **Variable Naming Rules**

* Variable names must start with a letter (a-z, A-Z) or an underscore (\_).
    
* The rest of the variable name can contain letters, digits (0-9), and underscores.
    
* Variable names are case-sensitive, meaning `age`, `Age`, and `AGE` are considered different variables.
    

### **Variable Usage**

You can use variables in various ways, such as in calculations, as part of strings, or in control structures like loops and conditionals:

```python
# Variable assignment
age = 30
name = "Hamza"
pi = 3.14
is_student = True
# Using variables in calculations
result = age * 2

# Using variables in strings (string concatenation)
greeting = "Hello, " + name

# Using variables in control structures
if is_student:
    print(name + " is a student.")
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698201297921/4f4f7334-8c15-45b6-bd84-d7094cebc701.png align="center")

## **Comments in Python**

Comments are used to add explanations or notes to your code. They are not executed by the Python interpreter and are purely for human readers. Python supports two types of comments:

### **Single-Line Comments**

You can create a single-line comment by using the `#` symbol. Everything after `#` on the same line is considered a comment.

```python
# This is a single-line comment

age = 30  # You can also add comments after code on the same line
```

Variables and comments are essential elements in Python programming that help you manage and document your code effectively. Let's explore them in detail:

## **Variables in Python**

In Python, variables are used to store and manage data. You can think of a variable as a named container that holds a value. Here's how you declare and use variables in Python:

### **Variable Declaration**

To declare a variable, you simply choose a name for it and assign a value using the assignment operator `=`. You don't need to explicitly specify the data type; Python infers it automatically.

```python
age = 30
name = "Hamza"
pi = 3.14
is_student = True
```

### **Variable Naming Rules**

* Variable names must start with a letter (a-z, A-Z) or an underscore (\_).
    
* The rest of the variable name can contain letters, digits (0-9), and underscores.
    
* Variable names are case-sensitive, meaning `age`, `Age`, and `AGE` are considered different variables.
    

### **Variable Usage**

You can use variables in various ways, such as in calculations, as part of strings, or in control structures like loops and conditionals:

```python
result = age * 2

# Using variables in strings (string concatenation)
greeting = "Hello, " + name

# Using variables in control structures
if is_student:
    print(name + " is a student.")
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698201430399/9412ead0-7bb3-4e77-92d5-88c92dc1fa53.png align="center")

## **Comments in Python**

Comments are used to add explanations or notes to your code. They are not executed by the Python interpreter and are purely for human readers. Python supports two types of comments:

### **Single-Line Comments**

You can create a single-line comment by using the `#` symbol. Everything after `#` on the same line is considered a comment.

```python
pythonCopy code# This is a single-line comment

age = 30  # You can also add comments after code on the same line
```

### **Multi-Line Comments (Docstrings)**

For longer comments or documentation, you can use triple-quotes (`'''` or `"""`) to create multi-line comments, also known as docstrings. These are often used to provide function or module documentation.

```python
'''
This is a multi-line comment or docstring.
It can span multiple lines.
'''
```

Comments are a valuable tool for making your code more understandable and maintainable, and they are considered a best practice in programming. They help you and other developers understand the purpose and functionality of your code.