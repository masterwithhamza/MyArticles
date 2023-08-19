---
title: "5# Understanding File Permissions and Ownership in Linux"
datePublished: Sat Aug 19 2023 09:00:09 GMT+0000 (Coordinated Universal Time)
cuid: cllhsgpvp000a09l062w1ca4m
slug: 5-understanding-file-permissions-and-ownership-in-linux
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1692267596815/511c9e3b-8412-46fc-bace-4029ddcf60f2.png
tags: devops, devops-articles, devops-journey, devopscommunity, hamzarehmansheikh4

---

In the world of DevOps, knowing how to manage who can access files and folders in Linux is super important. Imagine it like giving keys to different people to open different doors. This article will show you how to use these "keys" to keep your files safe and organized.

### **Who Can Open the Doors? Understanding Permissions:**

![Learning the shell - Lesson 9: Permissions](https://linuxcommand.org/images/file_permissions.png align="left")

In Linux, every file and folder has some rules about who can read, write, and use them. These rules are like passwords that decide who can do what.

1. **Read (r):** Imagine it like being able to look at the contents of a file, like reading a book.
    
2. **Write (w):** This is like having the power to change what's inside a file or create new things.
    
3. **Execute (x):** It's like having permission to use a program or go into a folder.
    

These permissions are shown as letters: r, w, and x. They're set for three groups: the owner of the file, the owner's group, and everyone else.

### **Who Owns the Keys? Understanding Ownership:**

![Linux File Ownership - javatpoint](https://static.javatpoint.com/linux/images/linux-file-ownership1.png align="left")

Every file also has an owner, like the main keyholder, and a group, like a bunch of people with similar keys.

1. `chown` **- Changing Ownership:** If you want to change who owns a file, you can use the `chown` command. For example, `sudo chown user:group filename` will change the owner and group.
    
2. `chgrp` **- Changing Group:** Use `chgrp` to change which group owns a file. You can do it like this: `sudo chgrp newgroup filename`.
    

### **Changing Passwords: Modifying Permissions:**

![File Permissions and chmod Command in Linux - CyberSophia](https://i0.wp.com/cybersophia.net/wp-content/uploads/2021/08/Linux.011.jpeg?fit=1920%2C1080&ssl=1 align="left")

* `chmod` **- Changing Permissions:** If you want to change the permissions of a file, you can use the `chmod` command. It's like changing passwords. You can use symbols like `+` and `-` and letters like `u` (user), `g` (group), and `o` (others).
    
* **Numbers Mode:** You can also use numbers to set permissions. Each number means something: 4 for read, 2 for write, and 1 for execute. For example, `chmod 755 filename` gives the owner full access and others can read and use.
    

### **Making Changes Everywhere: Recursively Changing Permissions:**

![How To Recursively Change The File's Permissions In Linux [CHMOD Linux]](https://itsubuntu.com/wp-content/uploads/2022/02/How-To-Recursively-Change-The-Files-Permissions-In-Linux.jpg align="left")

1. `-R` Flag: If you want to change permissions for a lot of files at once, you can use commands like `chmod` and `chown` with the `-R` flag. It's like changing all the passwords in a bunch of rooms.
    

### **Conclusion:**

Learning about file permissions and ownership is like learning how to give keys to the right people. With this knowledge, you can keep your files safe and organized in the Linux world of DevOps.