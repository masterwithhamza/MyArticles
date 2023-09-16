---
title: "Day11 # Working with VIM Text Editor"
datePublished: Sat Sep 16 2023 06:56:23 GMT+0000 (Coordinated Universal Time)
cuid: clmlodeux00060al789pg5xd2
slug: day11-working-with-vim-text-editor
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1694680635452/c864ce49-812a-4cfe-89f3-bd4e2a5b6c6a.png
tags: linux, devops, linux-for-beginners, devops-articles, masterwithhamza

---

Vim is an advanced text editor inspired by the Unix-based "Vi" text editor. Bram Moolenaar initially created Vim in 1991 as a response to the limitations of Vi while adding features that set it apart. Vim is particularly famous for its modal editing system, which allows users to switch between different modes for various tasks, making text manipulation exceptionally efficient.

## **Modes of Vim**

Vim operates in several modes, each serving a specific purpose:

1. **Normal Mode:** This is the default mode where you navigate and manipulate text. In Normal mode, you can move the cursor, copy, cut, paste, and perform various text editing tasks.
    
2. **Insert Mode:** When you want to insert or modify text, you enter Insert mode. This is similar to the way you'd work in a typical text editor.
    
3. **Visual Mode:** Visual mode allows you to select and manipulate text visually. You can select characters, lines, or blocks of text with ease.
    
4. **Command-Line Mode:** In this mode, you can enter commands to save, quit, search, replace, and perform other advanced actions.
    

Mastering these modes is crucial to becoming proficient with Vim.

### **Opening Vim**

To open Vim, open your terminal and type:

```bash
vim file1.txt
```

This will start Vim in Normal mode.

### **Basic Commands**

1. i
    

This is used to switch from Normal mode to Insert mode.

1. :w
    

This is used to save your file.

1. :q
    

This is used to exit Vim editor.

1. :wq
    

This is used to save and quit.

### **Navigating in Normal Mode**

1. h
    

This is used to move the cursor left.

1. j
    

This is used to move the cursor down.

1. k
    

This is used to move the cursor up.

1. l
    

This is used to move the cursor right.

1. 0
    

This is used to move the cursor to the beginning of the line.

1. $
    

This is used to move the cursor to the end of the line.

1. G
    

This is used to move the cursor to the end of the file.

1. gg
    

This is used to move the cursor to the beginning of the file.

### **Editing Text**

1. x
    

This is used to delete the character in the cursor.

1. dd
    

This is used to delete the current line.

1. yy
    

This is used to copy the current line.

1. p
    

This is used to paste text after the cursor.

1. u
    

This is used to undo the last change.

## **Conclusion**

Vim is a legendary text editor with a steep learning curve but incredible rewards for those who invest the time to master it. Its speed, flexibility, and efficiency make it a valuable tool for developers, sysadmins, and anyone who works with text. By following this guide and continually practising, you can unlock the full potential of Vim and take your text editing skills to the next level. Happy Vimming!