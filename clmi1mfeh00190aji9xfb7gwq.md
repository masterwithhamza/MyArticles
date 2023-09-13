---
title: "Day10 # Working with VI Text Editor"
datePublished: Wed Sep 13 2023 17:56:14 GMT+0000 (Coordinated Universal Time)
cuid: clmi1mfeh00190aji9xfb7gwq
slug: day10-working-with-vi-text-editor
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1694626594092/56ac968e-9e0b-425b-af4c-8b99b77819cf.png
tags: linux, devops, linux-for-beginners, devops-articles, masterwithhamza

---

VI, which stands for Visual Editor, was born in the late 1970s, and crafted by Bill Joy, co-founder of Sun Microsystems. It was designed as an improvement over earlier text editors like Ed and Ex and was initially released as part of the Berkeley Software Distribution (BSD) Unix. VI rapidly gained popularity thanks to its remarkable editing capabilities. In this comprehensive guide, we'll delve into the world of VI.

**Getting Started**

To open VI, simply open your terminal and type:

```bash
vi myfile.txt
```

This will open vi with an empty buffer, ready for you to start typing or editing text.

![How to Edit Files in Linux Using vi - dummies](https://www.dummies.com/wp-content/uploads/linux-vi.jpg align="left")

# **Navigation and Basic Editing**

1\. i

This is used to enter insert mode and start editing at the cursor.

2\. Esc

This is used to return to normal mode.

3\. h

This is used to move the cursor left.

4\. j

This is used to move the cursor down.

5\. k

This is used to move the cursor up.

6\. l

This is used to move the cursor right.

7\. w

This is used to move the cursor to the beginning of the next word.

8\. b

This is used to move the cursor to the beginning of the previous word.

9\. 0

This is used to move the cursor to the beginning of the line.

10\. $

This is used to move the cursor to the end of the line.

11\. G

This is used to move the cursor to the end of the file.

12\. gg

This is used to move the cursor to the beginning of the file.

# **Editing, searching and replacement**

1\. x

This is used to delete the character in the cursor.

2\. dd

This is used to delete the current line.

3\. yy

This is used to copy the current line.

4\. p

This is used to paste text after the cursor.

5\. P

This is used to past text before the cursor.

6\. u

This is used to undo the last change.

7\. :n

This is used to go to a new line.

8\. /search-term

This is used to search for "search-term" forward.

9\. ?search-term

This is used to search for "search-term" backwards.

10\. :s/old/new/g

This is used to replace the old with new on the current line.

11\. :%s/old/new/g

This is used to replace old with new globally in the file.

# **Saving, Exiting and Visual Mode**

1\. :w

This is used to save changes.

2\. :q

This is used to exit the vi editor.

3\. :wq

This is used to save changes and exit the vi editor.

4\. :q!

This is used to exit the vi editor without saving changes.

5\. v

This is used to select text character by character.

6\. V

This is used to select text line by line.

7\. ctrl + v

This is used to select rectangular blocks.

## **Conclusion**

VI and its modern incarnation, Vim, remain powerful and indispensable text editors, standing tall in the world of text editing. Whether you're a programmer, a writer, or a system administrator, VI's versatility and robust features make it a valuable addition to your toolkit. Dive in, start learning, and unlock the full potential of this venerable text editor.