---
title: "Lecture4 # Decision Making in Shell Scripting: The Power of Conditional Statements"
datePublished: Fri Oct 20 2023 16:52:24 GMT+0000 (Coordinated Universal Time)
cuid: clnyumuze000r0amg0350fp9q
slug: lecture4-decision-making-in-shell-scripting-the-power-of-conditional-statements
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1697820423555/8ab85c5b-cec8-4e6e-8c81-9dd7daedac7d.png
tags: linux, devops, shell-scripting, devops-articles, masterwithhamza

---

Shell scripting is not just about executing a sequence of commands; it's also about making intelligent decisions based on various conditions. Decision-making in shell scripting is achieved through conditional statements. In this article, we'll explore the use of conditional statements in shell scripts to control the flow of execution and perform different actions depending on specific conditions.

## **Conditional Statements in Shell Scripting**

Conditional statements in shell scripting allow you to create rules that determine which commands or actions to execute based on certain conditions.

## **The 'if' Statement**

```bash
#!/bin/bash

number=15

if [ $number -gt 10 ]; then
    echo "The number is greater than 10."
fi
```

In this script, if the condition `$number -gt 10` is true, it will print "The number is greater than 10."

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698121865645/a9d2b984-7933-439e-86ad-61df07a89cf2.png align="center")

## **The 'if-else' Statement**

The 'if-else' statement extends the 'if' statement to handle an alternative action when the condition is false:

```bash
#!/bin/bash

username="hamza"

if [ "$username" == "hamza" ]; then
    echo "Access granted."
else
    echo "Access denied."
fi
```

**Output:**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698149335591/45d06e79-489e-47cc-bb14-a828a3b5193b.png align="center")

## **The 'elif' Statement**

When you have multiple conditions to check, you can use 'elif' to evaluate them one by one. The script executes the code block of the first true condition it encounters:

```bash
grade="A"
if [ "$grade"=="A" ]; then
    echo "congratulation hamza you got A Grade"
elif [ "$grade"=="B" ]; then
    echo "hamza, you got B grade"
else
    echo "failed"
fi
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698149707039/428ba75f-213d-4d3f-b459-75098e45be0c.png align="center")

## **Conclusion**

Conditional statements are a fundamental part of shell scripting, allowing you to create intelligent scripts that make decisions based on various conditions. Whether you need to perform different actions for different scenarios, handle multiple options, or control the flow of your script, mastering the use of 'if,' 'if-else,' and 'elif,' statements will greatly enhance your scripting capabilities. With these tools, you can create more powerful and versatile shell scripts to automate complex tasks and respond to different situations effectively.