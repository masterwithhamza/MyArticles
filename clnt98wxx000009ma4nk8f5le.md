---
title: "Lecture10 # Lists and Sets in Python for Beginners"
datePublished: Mon Oct 16 2023 18:54:51 GMT+0000 (Coordinated Universal Time)
cuid: clnt98wxx000009ma4nk8f5le
slug: lecture10-lists-and-sets-in-python-for-beginners
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1697482455773/194ca801-775e-4f17-9d5d-8f59acd62b7e.png
tags: python, devops, python-beginner, devops-articles, masterwithhamza

---

Lists and sets are two popular data structures in Python that allow you to store and manipulate collections of items. In this beginner-friendly guide, we'll explore lists and sets, including how to create and manipulate them, and when to use each of them in your Python programs.

## **Lists in Python**

A list is a collection of values, often of different data types, that are ordered and mutable. Lists are created by enclosing a comma-separated sequence of items in square brackets `[ ]`. Here's how you can work with lists:

### **Creating Lists**

```python
my_list = [1, 2, 3, 'apple', 'banana', 'cherry']
```

In this example, `my_list` is a list containing integers and strings.

### **Accessing List Elements**

You can access elements in a list using index positions, starting from 0 for the first item. Negative indices count from the end of the list.

```python
first_item = my_list[0]      # Access the first item (1)
last_item = my_list[-1]      # Access the last item ('cherry')
```

## **Sets in Python**

A set is an unordered collection of unique elements. Sets are created by enclosing a comma-separated sequence of items in curly braces `{ }` or by using the `set()` constructor. Here's how you can work with sets:

### **Creating Sets**

```python
my_set = {1, 2, 3, 2, 4, 5}
```

In this example, `my_set` contains unique elements, so the duplicate '2' is automatically removed.

### **Accessing Set Elements**

Sets do not support indexing, so you cannot directly access elements by their position. Instead, you use set operations like `in` to check if an element exists in the set.

```python
is_present = 3 in my_set      # Check if 3 is in the set (True)
```

## **When to Use Lists or Sets**

* Use **lists** when you need to maintain order and may have duplicate elements.
    
* Use **sets** when you need to store unique elements and order doesn't matter. Sets are also useful for checking membership efficiently.
    

## **Conclusion**

Lists and sets are versatile data structures in Python, each with its unique characteristics and use cases. Understanding when to use lists or sets and how to create, access, and manipulate them is essential for effective Python programming. With this knowledge, you'll be well-equipped to work with collections of data in your Python programs.