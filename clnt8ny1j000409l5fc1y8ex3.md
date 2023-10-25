---
title: "Lecture8 # Error Handling with Try-Except"
datePublished: Mon Oct 16 2023 18:38:32 GMT+0000 (Coordinated Universal Time)
cuid: clnt8ny1j000409l5fc1y8ex3
slug: lecture8-error-handling-with-try-except
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1697481467614/4832442d-bdc0-412c-887f-276d847aa9ed.png
tags: python, devops, python-beginner, devops-articles, masterwithhamza

---

Error handling with `try` and `except` is a crucial aspect of Python programming that allows you to handle exceptions and prevent your program from crashing when it encounters unexpected errors. It's a way to gracefully manage and recover from exceptional conditions.

**My Python codes:** [https://masterwithhamza@bitbucket.org/hamxaflutterapps/mypythoncodes.git](https://masterwithhamza@bitbucket.org/hamxaflutterapps/mypythoncodes.git)

In Python, you use a `try` block to enclose code that might raise an exception. You then follow it with one or more `except` blocks that specify how to handle different types of exceptions. If an exception occurs within the `try` block, Python checks if there's a corresponding `except` block for that exception. If one is found, the code inside the `except` block is executed.

Here's the basic structure:

```python
try:
    # Code that might raise an exception
except ExceptionType:
    # Code to handle the exception
```

* `try`: Encloses the code where an exception might occur.
    
* `except ExceptionType`: Specifies the type of exception to handle. You can catch specific exceptions or a more general `Exception` class.
    

```python
try:
    number = int(input("Enter a number: "))
    result = 10 / number
    print("Result is:", result)
except ZeroDivisionError:
    print("Error: Cannot divide by zero.")
except ValueError:
    print("Error: Invalid input. Please enter a valid number.")
```

In this example, the `try` block attempts to get user input, perform a division operation, and print the result. If the user enters zero, it raises a `ZeroDivisionError`. If the user enters something that's not a number, it raises a `ValueError`. The corresponding `except` blocks handle each of these exceptions gracefully.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698201841797/b451e57c-d275-4396-87c7-54efc92b4e8b.png align="center")

## **Conclusion**

Error handling with `try` and `except` is an essential aspect of writing robust Python programs. It allows you to anticipate and manage exceptions, making your code more reliable and user-friendly. As you gain more experience in Python, you'll develop a better understanding of when and how to use error handling effectively in your programs.