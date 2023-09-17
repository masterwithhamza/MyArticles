---
title: "Day13 # Guide to Working with Text Files (Basic Commands)"
datePublished: Sun Sep 17 2023 04:25:45 GMT+0000 (Coordinated Universal Time)
cuid: clmmyfjjg000609jk7ludgmrw
slug: day13-guide-to-working-with-text-files-basic-commands
tags: linux, devops, linux-for-beginners, devops-articles, masterwithhamza

---

Linux, the open-source operating system celebrated for its flexibility and control, offers a robust set of tools and commands for working with files. Whether you're a system administrator, programmer, or an everyday user, understanding how to navigate, manipulate, and manage files is a fundamental skill. In this article, we'll embark on a journey through the world of file management in Linux.

1\. touch

This command is used to create an empty file or update the timestamp of a file without modifying its content.

2\. touch -t 202303041300 file1

This command is used only to affect the access and modification timestamp not the content of the file.

3\. cat

This command is used for viewing the content of any file. this is also used for concatenating the contents of different files.

4\. cat -n file1

This command is used for displaying the content of the file with a line number added to each line.

5\. less

This command is used for viewing larger log files and configuration [files. It](http://files.it) allows you to read through them step by step and find the information you need efficiently.

6\. less +G file1

This command is used to show the last page of the content.

7\. head

This command is used to show the first ten lines of the file but you can specify a different number of lines to be displayed if needed.

8\. head -c 100 file1

This command is used to show the first 100 characters of a file.

9\. tail

This command is used to show the last ten lines of a file but you can specify a different number of lines to be displayed if needed.

10\. tail -f file1

This command is used to monitor the last few lines of a file in real-time as new content is appended to it.

11\. sort

This command is used to sort the lines of a text file. sort will arrange the lines in ascending order.

12\. sort -u file3

This command is used to sort the lines of a file and remove the duplicates in the file.

13\. wc

This command is used to count the number of lines, words and characters in a file.

14\. fold

This command is used to wrap the lines of a text file to a specific width.

15\. comm

This command is used to compare two sorted files line by line and display the lines that are common to both files as well as the lines that are unique to each file.

## **Conclusion**

File management is a fundamental skill for anyone using Linux. Whether you're organizing your files, maintaining a web server, or developing software, understanding these file operations and the underlying permissions system is essential. By mastering these basics, you'll have the tools to efficiently manage files in the Linux environment, enabling you to harness the full potential of this powerful operating system.