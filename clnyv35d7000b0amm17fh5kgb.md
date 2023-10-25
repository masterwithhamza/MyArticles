---
title: "Lecture5 # Repetitive Structures in Shell Scripting: Loops for Efficiency"
datePublished: Fri Oct 20 2023 17:05:04 GMT+0000 (Coordinated Universal Time)
cuid: clnyv35d7000b0amm17fh5kgb
slug: lecture5-repetitive-structures-in-shell-scripting-loops-for-efficiency
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1697821159454/984de86c-f191-45ff-b75e-bac02bfce5c5.png
tags: linux, devops, shell-scripting, devops-articles, masterwithhamza

---

In shell scripting, repetitive structures, often referred to as loops, are essential tools for performing the same set of actions multiple times. Whether you want to process files, perform calculations, or interact with a list of items, loops enable you to automate tasks efficiently. This article will introduce you to two of the most commonly used loops in shell scripting: the "for" loop and the "while" loop.

## **The "for" Loop**

The "for" loop is a structured way to repeat a set of commands a specified number of times or to iterate over a list of items, such as files or values in an array.

```bash
#!/bin/bash

for number in 1 2 3 4 5
do
    echo $number
done
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698199490686/1f5964b6-fc09-4948-b2d2-502b01c4bdeb.png align="center")

You can also use a "for" loop to iterate over a list of items, such as files in a directory:

```bash
#!/bin/bash

for file in $(ls /path/to/directory)
do
    echo "Processing file: $file"
    # Add your processing commands here
done
```

In this example, the "for" loop iterates over the files in the specified directory and acts on each file.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698199750913/196e8450-6713-467a-a6ea-4e7db5c85696.png align="center")

## **The "while" Loop**

The "while" loop allows you to execute a set of commands as long as a specified condition is true.

```bash
#!/bin/bash

count=1

while [ $count -le 5 ]
do
    echo $count
    ((count++))
done
```

You can use a "while" loop to process data until a certain condition is met, making it suitable for tasks where the number of iterations is unknown in advance.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698200510387/a194713c-9bf3-49e9-a0fb-124e592c33b6.png align="center")

## **Conclusion**

Repetitive structures, such as "for" and "while" loops, are powerful tools in shell scripting that help you automate repetitive tasks and handle a wide range of scenarios. By understanding how to use these loops, you can process lists of items, repeat actions a certain number of times, or execute commands as long as specific conditions are met. Mastery of these looping constructs allows you to create efficient and flexible shell scripts for a variety of tasks, making your scripting endeavours more productive and powerful.