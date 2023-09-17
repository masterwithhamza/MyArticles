---
title: "Day12 # A Guide to Working with Directories"
datePublished: Sun Sep 17 2023 04:10:35 GMT+0000 (Coordinated Universal Time)
cuid: clmmxw1k7000009mn8h3u8itj
slug: day12-a-guide-to-working-with-directories
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1694922893230/66b81046-ed82-4d26-b5fb-d9841c670a82.png
tags: linux, devops, linux-for-beginners, devops-articles, masterwithhamza

---

At the core of Linux's file system is the root directory, denoted by a forward slash (`/`). Everything in Linux stems from this root directory, forming a tree-like structure. Let's explore some essential directory-related commands and concepts.

1\. mkdir

This command is used to create a new directory.

2\. cd

This command is used to change the directory.

2\. cd ..

This command is used to go back from the current directory to the parent directory.

3\. cd -

This command is used to switch your current directory to the directory you were in before executing the last cd command.

4\. tree

This command is used to display the directory structure of a file system in a tree-like format.

5\. ls -a

This command is used to display the files and directories in the current directory including those whose names start with a dot (.) which typically indicate hidden files or directories in the system.

6\. ls -l

This command is used to display a detailed list of the files and directories in the current directory.

7\. ls -al

This command is used to display a detailed list of files and directories as well as hidden files and directories in the current directory.

8\. ls -tl

This command is used to display a list of contents of the current directory with their modification time.

9\. ls -sl

This command is used to display the content of the current directory in detail and show the size of each file and directory in blocks.

10\. ls -slh

This command is used to list the content in a long format with the size displayed in a human-readable format (kb, MB).

11\. mkdir

This command is used to create a new directory.

12\. mkdir -p hamza/age

This command is used if the present directory does not already exist the command will create them as well ensuring that the entire path is created.

13\. rmdir

This command is used to remove the empty directory.

14\. rm -r hamza

This command is used to remove the file and folder recursively.

15\. rm -rf hamza

This command is used to remove the file and directories forcefully.

16\. cp

This command is used to copy the file and directories from source to desgination.

17\. mv

This command is used to cut files and directories from source to desgination.

## **Conclusion**

Directories are the backbone of Linux's file system structure, allowing you to organize and access your files efficiently. By mastering basic directory operations you'll have a solid foundation for working with Linux. Whether you're a sysadmin managing a server, a developer coding in a Linux environment, or an everyday user exploring the possibilities of this versatile OS, these directory skills are essential for your Linux journey.