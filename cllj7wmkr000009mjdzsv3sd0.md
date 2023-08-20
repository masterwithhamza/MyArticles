---
title: "6# Getting Started with Shell Scripting"
datePublished: Sun Aug 20 2023 09:00:11 GMT+0000 (Coordinated Universal Time)
cuid: cllj7wmkr000009mjdzsv3sd0
slug: 6-getting-started-with-shell-scripting
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1692295846756/8a0b6637-90b4-4230-9048-3ba3e026df00.png
tags: devops, devops-articles, devops-journey, devopscommunity, hamzarehmansheikh4

---

Shell scripting is your gateway to automation in the world of DevOps. Imagine having a magic wand to perform repetitive tasks with a single command! In this beginner-friendly guide, we'll embark on an exciting journey into the realm of shell scripting. Buckle up, and let's uncover the power of scripting for automating tasks, enhancing productivity, and making your DevOps journey smoother.

### **Why Shell Scripting Matters:**

Shell scripting is like giving instructions to your computer using simple text commands. It's not about writing complex code; it's about making your computer do things automatically. Whether it's setting up servers, deploying applications, or managing files, shell scripting simplifies your tasks.

### **Choosing Your Shell:**

Different types of shells are like different languages your computer understands. The two main shells are Bash (Bourne-Again SHell) and Zsh (Z Shell). For beginners, Bash is a great starting point due to its widespread use and ease of learning.

### **Creating Your First Script:**

* **Opening a Text Editor:** You can use simple text editors like Notepad (Windows) or nano (Linux/Mac) to write your script.
    
* **Writing Your Commands:** Start with basic commands like `echo`, which displays text, or `ls`, which lists files. For example, type `echo "Hello, DevOps!"`.
    
* **Saving Your Script:** Save the file with a `.sh` extension, like `my_script.sh`.
    

### **Making Your Script Executable:**

1. **Using** `chmod` **Command:** To run your script, you need to make it executable. In the terminal, type `chmod +x my_script.sh`.
    
2. **Running Your Script:** Now you can run your script by typing `./my_script.sh`. Your computer will follow the commands you wrote.
    

### **Variables and Inputs:**

* **Creating Variables:** Variables store information. For example, `name="Alice"`.
    
* **Using Variables:** You can use variables in your script by adding `$` before the variable name. For example, `echo "Hello, $name!"`.
    
* **User Inputs:** You can ask the user for input using the `read` command. For example, `read -p "Enter your name: " username`.
    

### **Conditional Statements:**

**IF Statements:** IF statements help your script make decisions. For example:

```bash
if [ "$age" -ge 18 ]; then
    echo "You're an adult."
else
    echo "You're a minor."
fi
```

### **Looping with Loops:**

**FOR Loops:** FOR loops repeat a set of commands. For example:

```bash
for i in 1 2 3; do
    echo "Number: $i"
done
```

### **Conclusion:**

Shell scripting is your ally in the DevOps realm. It empowers you to automate tasks, save time, and eliminate errors. As you delve deeper, you'll discover endless possibilities for enhancing your efficiency and boosting your productivity in the world of DevOps.