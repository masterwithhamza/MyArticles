---
title: "Day17 # File Ownership and Permissions in Linux"
datePublished: Sun Sep 24 2023 09:17:58 GMT+0000 (Coordinated Universal Time)
cuid: clmx8yaz5000808l21r1kfafp
slug: day17-file-ownership-and-permissions-in-linux
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1695546998162/07a3e336-512a-435b-b7d1-362e30dc40f6.png
tags: linux, devops, linux-for-beginners, devops-articles, masterwithhamza

---

In the world of Linux and Unix-based operating systems, file ownership and permissions are fundamental concepts that govern who can access and manipulate files and directories. Understanding how these mechanisms work is essential for both system administrators and regular users. In this detailed article, we will explore file ownership and permissions in Linux.

## **Ownership in Linux**

In Linux, each file and directory is associated with an owner and a group. These ownership attributes determine who has control over the file and what they can do with it.

### **1\. User (Owner)**

* **User**: The user who created the file or directory is the owner.
    
* **UID**: Each user is assigned a unique User ID (UID), a numeric identifier.
    
* **File Control**: The owner can read, write, and delete the file. For directories, the owner can also create, rename, and delete files within it.
    

### **2\. Group**

* **Group**: Files and directories belong to a specific group.
    
* **GID**: Each group is assigned a unique Group ID (GID), a numeric identifier.
    
* **Group Control**: Group members (users) can access files and directories based on group permissions.
    

### **3\. Others**

* **Others**: Everyone else on the system falls into the "others" category.
    
* **World Control**: Others can access files and directories based on permissions set for this category.
    

## **Permissions in Linux**

Linux uses a permission system that consists of three types of access: read, write, and execute. Each type of access can be granted or denied to the owner, group, and others, resulting in a total of nine permission bits for each file or directory.

### **1\. Read (r)**

* **File**: Allows reading the file's contents.
    
* **Directory**: Allows listing the directory's contents.
    

### **2\. Write (w)**

* **File**: Allows modifying the file's contents or deleting it.
    
* **Directory**: Allows creating, deleting, or renaming files within the directory.
    

### **3\. Execute (x)**

* **File**: Allows executing the file as a program or script.
    
* **Directory**: Allows accessing (entering) the directory.
    

## **Viewing Permissions**

You can view the ownership and permissions of files and directories using the `ls -l` command:

```bash
ls -l /path/to/file_or_directory
```

This command displays detailed information about the file or directory, including ownership and permissions. Here's an example output:

```bash
-rw-r--r-- 1 user1 group1 1234 Sep 24 15:30 file.txt
```

* The first field shows file type and permissions (`-rw-r--r--`).
    
* The second field indicates the number of hard links to the file (usually 1).
    
* The third and fourth fields display the owner and group (user1 and group1).
    
* The fifth field shows the file size (in bytes).
    
* The last fields display the modification date and file/directory name.
    

## **Modifying Permissions**

You can change file and directory permissions using the `chmod` command. The basic syntax is as follows:

```bash
chmod [options] mode file_or_directory
```

* `[options]`: Additional options like `-R` for recursive changes.
    
* `mode`: A three-digit octal number that represents the desired permissions.
    
* `file_or_directory`: The path to the file or directory whose permissions you want to change.
    

### **Octal Mode**

* Each digit in the octal mode represents a different user category: owner, group, and others.
    
* Each digit is a sum of its corresponding permissions: read (4), write (2), and execute (1).
    
* The octal mode is calculated by adding these sums. For example:
    
    * `chmod 755 file.txt` gives read, write, and execute permission to the owner, and read and execute permissions to the group and others.
        

### **Symbolic Mode**

* You can also use symbolic mode with the `chmod` command. It allows you to modify permissions symbolically, using letters like `u` for user (owner), `g` for group, and `o` for others, along with operators like `+` (add) and `-` (remove).
    
* For example: `chmod u+w file.txt` adds write permission for the owner.
    

## **Changing Ownership**

To change the owner and group of a file or directory, use the `chown` and `chgrp` commands, respectively:

```bash
chown new_owner:new_group file_or_directory
```

```bash
chgrp new_group file_or_directory
```

* `new_owner` and `new_group` are the desired new owner and group names.
    
* You may need to use `sudo` to change ownership, as these commands require administrative privileges.
    

## **Common Examples**

Here are some common examples to illustrate the use of file ownership and permissions:

### **1\. Restricting File Access**

Suppose you have a sensitive document named `secret.txt`, and you want to restrict access to it:

```bash
chmod 600 secret.txt
```

This command sets read and write permissions for the owner (you) while denying any access to the group and others.

### **2\. Sharing Files Within a Group**

You're working on a project with a group named `project_team`, and you want to share a directory with the team:

```bash
chmod 770 project_directory
chown :project_team project_directory
```

This sets read, write, and execute permissions for both the owner and the group while denying access to others. It also assigns the group `project_team` as the group owner of the directory.

### **3\. Executing Scripts**

If you have a script named [`myscript.sh`](http://myscript.sh) that you want to execute, you can add execute permissions for the owner:

```bash
chmod u+x myscript.sh
```

This command allows the owner to run the script.

## **Conclusion**

File ownership and permissions in Linux are a fundamental aspect of security and access control. By understanding how ownership and permissions work and by following best practices, you can maintain a secure and organized file system while allowing users and processes the appropriate levels of access to files and directories. Properly managing ownership and permissions is key to a well-maintained and secure Linux environment.