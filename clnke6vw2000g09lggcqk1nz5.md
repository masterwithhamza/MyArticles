---
title: "Lecture3 # Data Types in Python"
datePublished: Tue Oct 10 2023 14:03:19 GMT+0000 (Coordinated Universal Time)
cuid: clnke6vw2000g09lggcqk1nz5
slug: lecture3-data-types-in-python
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1696946557628/7603d4de-b436-4bcf-9bc5-944f356d678a.png
tags: python, devops, marketing, python-beginner, devops-articles

---

In Python, data types are used to categorize and represent different types of values that you can manipulate in your programs. Understanding data types is essential because they determine how you can use and operate on your data. Python provides a variety of built-in data types, and here are some of the most common ones:

1. **Integer (**`int`**)**
    
    * Represents whole numbers (positive or negative) without a decimal point.
        
    * Example: `42`, `-10`, `0`
        
2. **Float (**`float`**)**
    
    * Represents real numbers with a decimal point.
        
    * Example: `3.14`, `-0.5`, `2.0`
        
3. **String (**`str`**)**
    
    * Represents sequences of characters enclosed in single (' ') or double (" ") quotes.
        
    * Example: `"Hello, Python!"`, `'12345'`, `"Data Types"`
        
4. **Boolean (**`bool`**)**
    
    * Represents the truth values `True` or `False`.
        
    * Used for making decisions and logical operations.
        
    * Example: `True`, `False`
        
5. **List**
    
    * An ordered collection of items that can be of different data types.
        
    * Enclosed in square brackets `[]`.
        
    * Example: `[1, 2, 3]`, `['apple', 'banana', 'cherry']`
        
6. **Tuple**
    
    * Similar to lists, but they are immutable (cannot be changed after creation).
        
    * Enclosed in parentheses `()`.
        
    * Example: `(1, 2, 3)`, `('John', 25)`
        
7. **Dictionary (**`dict`**)**
    
    * A collection of key-value pairs.
        
    * Enclosed in curly braces `{}`.
        
    * Example: `{'name': 'Alice', 'age': 30, 'city': 'New York'}`
        
8. **Set**
    
    * An unordered collection of unique elements.
        
    * Enclosed in curly braces `{}` or created using the `set()` constructor.
        
    * Example: `{1, 2, 3}`, `set([2, 2, 3, 3, 4])`
        
9. **NoneType (**`None`**)**
    
    * Represents the absence of a value or a null value.
        
    * Often used to indicate that a variable has no assigned value.
        
10. **Complex (**`complex`**)**
    
    * Represents complex numbers with both real and imaginary parts.
        
    * Written as `a + bj`, where `a` and `b` are real numbers, and `j` represents the square root of -1.
        
    * Example: `3 + 4j`, `-2.5 - 1.7j`
        

These data types are the building blocks of Python programs, and you can perform various operations on them, such as arithmetic operations on numbers, concatenation and manipulation of strings, indexing and slicing of sequences (lists, tuples, strings), and more.

You can also create your custom data types using classes, but understanding and using these built-in data types is fundamental for any Python programmer. Additionally, Python is a dynamically typed language, which means you don't need to declare the data type of a variable explicitly; it is inferred at runtime based on the value assigned to it.