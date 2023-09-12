---
title: "Day6 # Setup first virtual machine on Amazon EC2 Instance"
datePublished: Tue Sep 12 2023 04:49:36 GMT+0000 (Coordinated Universal Time)
cuid: clmfu2yaf000b09l8h6x8ekwr
slug: day6-setup-first-virtual-machine-on-amazon-ec2-instance
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1694491214835/1d93c7f0-07ad-4a4b-a416-9996ac5636bf.png
tags: linux, devops, linux-for-beginners, devops-articles, masterwithhamza

---

Amazon Elastic Compute Cloud (Amazon EC2) is a cloud computing service that allows you to create and run virtual machines (instances) in the Amazon Web Services (AWS) cloud. In this article, we will guide you through the process of launching and configuring your first EC2 instance.

### **Step 1:**

Ensure you have an AWS account. If not, you can create one at [**AWS Sign-up**](https://aws.amazon.com/). Log in to the AWS Management Console using your AWS account credentials.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694491587502/a8467ec0-eb13-4feb-bc6e-c55ad74eaf28.png align="center")

### Step 2:

Once logged in, navigate to the EC2 Dashboard by clicking on the "Services" menu and selecting "EC2" under the "Compute" section.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694491740017/c7d9b676-d1be-4892-9b2a-e6af4ad8f650.png align="center")

### **Step 3:**

Then Click on instances.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694491881629/f390b477-04f9-4f59-b326-f8b204c6b6fc.png align="center")

### Step 4:

Then click on Launch instances.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694491946485/dffe92e1-64b5-4cac-b8ef-b8b8ed9f42e4.png align="center")

### Step 5:

So now first of all give the name to your virtual machine.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694492089379/15a5f872-50da-4c38-9b35-72bb7b784532.png align="center")

### Step 6:

Then scroll down and select the operating system for your virtual machine. In my case, I am selecting the Ubuntu.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694492217747/4b33e359-0a83-4468-b774-b4120464c9a4.png align="center")

### Step 7:

Now scroll down and select the type of your instance. In my case, I am selecting t2.micro because it's free.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694492328948/83480e7b-60f7-4c3b-aa12-60050b9d0dd5.png align="center")

### Step 8:

Ensure that you have access to the selected key pair before you launch the instance. so Scroll down and click on Create New key pair.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694492422535/a1223801-eab3-4e51-a5ce-4733fc3500a7.png align="center")

### Step 9:

Then enter the key pair name and click on the create key pair button. so your key will be downloaded automatically.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694492564394/f04f2984-5fb7-4b7e-b6a8-4abc0f05eb7a.png align="center")

### Step 10:

Then scroll down and check out these 2 options.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694492684890/46e8c6ea-c402-4764-bc36-ffb3d096e461.png align="center")

### Step 11:

So now click on the Lunch instance button.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694492772450/22e15b3d-512b-4024-a600-27a939a32259.png align="center")

So your instance is launching.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694492808481/d6b8aaf8-2c0e-4696-a356-8242999b37a5.png align="center")

### Step 12:

So now go to instances. Congratulations your instance is successfully created and running.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694492903125/a45d3c6a-e6e1-4d19-958c-dc247baac02c.png align="center")

### Step 13 :

Now if you want to connect to your instance then Select your instance and click on connect.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694493072113/0cb70378-0e91-4d5c-b652-15e2960e0f78.png align="center")

so now scroll down and click on the connect button.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694493134504/b23d1d1b-cfef-4286-9736-5d2a371799cb.png align="center")

### Step 14 :

Congratulations your instance connects successfully now you can work on your virtual machine.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1694493223087/1a04b133-8da7-45f9-aef3-15ee5b9c7f37.png align="center")

### Some Essential Commands in Linux

1. **Clear:**
    

This command is used to clear your terminal.

1. `pwd` **- Print Working Directory:**
    

* Displays the current working directory (the directory you are currently in).
    

1. `cd` **- Change Directory:**
    

* Used to change your current directory. For example, `cd /path/to/directory` will change to the specified directory.
    

1. `mkdir` **- Make Directory:**
    

* Creates a new directory. For example, `mkdir myfolder` will create a directory named "myfolder."
    

1. `touch` **- Create Empty File:**
    

* Creates an empty file. For example, `touch myfile.txt` will create a file named "myfile.txt."
    

1. `rm` **- Remove Files or Directories:**
    

* Deletes files or directories. Be cautious with this command, as it doesn't move items to a trash/recycle bin; they are deleted permanently. For example, `rm myfile.txt` removes a file.
    

1. `history` - **View Command History:**
    

Shows a list of previously executed commands.