---
title: "Lecture7 # Conditional Statements (if/else)"
datePublished: Tue Oct 10 2023 14:58:23 GMT+0000 (Coordinated Universal Time)
cuid: clnkg5pgk000b09jvdmpyfvqu
slug: lecture7-conditional-statements-ifelse
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1696949863708/587f3073-ac26-4955-8b23-6848b596a859.png
tags: python, devops, python-beginner, devops-articles, masterwithhamza

---

Conditional statements, such as `if` and `else` statements, are fundamental building blocks of programming that allow you to make decisions in your code based on certain conditions. In Python, these statements help control the flow of your program by executing different code blocks depending on whether specific conditions are true or false.

Here's a beginner-friendly guide to understanding `if` and `else` statements in Python:

**My Python codes:** [https://masterwithhamza@bitbucket.org/hamxaflutterapps/mypythoncodes.git](https://masterwithhamza@bitbucket.org/hamxaflutterapps/mypythoncodes.git)

## **The** `if` Statement

The `if` statement is used to test a condition. If the condition evaluates to `True`, the code block inside the `if` statement is executed. If the condition is `False`, the code block is skipped. Here's the basic structure:

```python
if condition:
    # Code to be executed if the condition is True
```

### **Example:**

```python
age = 18

if age >= 18:
    print("You are an adult.")
```

In this example, if the `age` is greater than or equal to 18, the message "You are an adult." will be printed.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698201690186/9d2e5317-85bb-49f7-94ff-d5fc98d8a7ce.png align="center")

## **The** `else` Statement

The `else` statement is used in conjunction with an `if` statement to provide an alternative code block to execute when the `if` condition is `False`. Here's how it works:

```python
if condition:
    # Code to be executed if the condition is True
else:
    # Code to be executed if the condition is False
```

### **Example:**

```python
age = 15

if age >= 18:
    print("You are an adult.")
else:
    print("You are a minor.")
```

In this example, if the `age` is less than 18, the message "You are a minor." will be printed because the condition in the `if` statement is `False`.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698201720142/d7e2253a-10af-41cc-8db0-1c0a39f01ec4.png align="center")

## **The** `elif` Statement

The `elif` statement (short for "else if") allows you to test multiple conditions in sequence. It's used when you have more than two possible outcomes. Here's how it works:

```python
if condition1:
    # Code to be executed if condition1 is True
elif condition2:
    # Code to be executed if condition2 is True
else:
    # Code to be executed if neither condition1 nor condition2 is True
```

### **Example:**

```python
grade = 85

if grade >= 90:
    print("A")
elif grade >= 80:
    print("B")
elif grade >= 70:
    print("C")
else:
    print("D")
```

In this example, the program evaluates the grade and prints the corresponding letter grade based on the conditions.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698201748066/9f2d4a5d-34a0-42d9-818b-e5b253d71267.png align="center")

## **Conclusion**

Conditional statements (`if`, `else`, `elif`) are essential for controlling the flow of your Python programs. They allow your code to make decisions based on conditions, making your programs more dynamic and responsive to different scenarios. As you gain more experience in Python programming, you'll find that conditional statements are used extensively in many applications and algorithms.