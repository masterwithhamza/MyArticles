---
title: "Lecture6 # Accepting User Input in Python"
datePublished: Tue Oct 10 2023 14:46:59 GMT+0000 (Coordinated Universal Time)
cuid: clnkfr1td001709lg8de3h84a
slug: lecture6-accepting-user-input-in-python
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1696949181411/fe63123a-0a1a-4e80-9e89-aef0b4e5a34c.png
tags: python, devops, python-beginner, devops-articles, masterwithhamza

---

Accepting user input is a common task in Python, and it allows your programs to interact with users by taking data from them. You can use the `input()` function to read user input from the keyboard. Here's a step-by-step guide on how to accept user input in Python:

**My Python codes:** [https://masterwithhamza@bitbucket.org/hamxaflutterapps/mypythoncodes.git](https://masterwithhamza@bitbucket.org/hamxaflutterapps/mypythoncodes.git)

**Using the** `input()` **Function:**

The `input()` function reads a line of text entered by the user and returns it as a string. Here's a simple example:

```python
# Accepting user input
user_input = input("Enter your name: ")
```

1. In this example, the `input()` function displays the message "Enter your name: " to the user, and the user can type their name. The entered text is then stored in the `user_input` variable as a string.
    
2. **Converting User Input to Other Data Types:**
    
    By default, `input()` returns a string. If you want to work with the input as a different data type, like an integer or a float, you'll need to convert it using functions like `int()` or `float()`:
    

```python
# Accepting and converting user input to an integer
age_str = input("Enter your age: ")
age = int(age_str)
```

1. In this example, we first accept the user input as a string, and then we use `int()` to convert it to an integer.
    
2. **Using User Input in Your Program:**
    
    Once you've captured user input, you can use it in your program as needed. For example, you can print it, perform calculations, or use it in conditionals:
    

```python
print("Hello, " + user_input + "!")  # Printing a greeting
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698201634073/710e8339-25e5-45e8-8e20-e1ed8d628539.png align="center")

That's how you can accept user input in Python. It's a powerful way to make your programs interactive and dynamic, and it opens up countless possibilities for creating user-friendly applications.