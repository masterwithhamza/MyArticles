---
title: "Lecture4 #Git Advanced Techniques: Rebasing, Commit History, Tagging, Reset, and Ignore"
datePublished: Thu Oct 26 2023 03:16:58 GMT+0000 (Coordinated Universal Time)
cuid: clo6m5b8m000109mfe6g0hjqp
slug: lecture4-git-advanced-techniques-rebasing-commit-history-tagging-reset-and-ignore
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1698289273900/2bc087df-555e-419d-a503-a969691a9fc7.png
tags: github, git, devops, devops-articles, masterwithhamza

---

Git offers advanced techniques to help developers manage their projects more effectively. In this article, we will explore some of these advanced Git concepts, including rebasing, viewing commit history, tagging for releases, resetting changes and commits, and ignoring files and directories.

**1\. Rebasing: Rewriting Commit History with Rebasing**

Rebasing is a powerful feature in Git that allows you to reorganize your commit history by moving, combining, or removing commits. This can result in a cleaner and more linear history. To rebase a branch:

* Use the `git rebase` command, followed by the branch you want to rebase onto (often the main branch):
    

```bash
git rebase master
```

* Git will pause the rebase process if there are conflicts. Resolve the conflicts as you would during a merge.
    
* After resolving conflicts, continue the rebase with `git rebase --continue`.
    
* When the rebase is complete, your branch will have the updated commit history.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698289680355/95f00943-468b-4ff4-8dc8-c7a965c5f14e.png align="center")

**2\. Git Log: Viewing the Commit History**

The `git log` command allows you to view the commit history of your repository. By default, it displays a list of commits with their SHA-1 hashes, authors, dates, and commit messages. You can use various options to customize the log output, such as limiting the number of commits or formatting the log to your preferences.

For a basic log display, simply run:

```bash
git log
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698289742405/d6a66080-7df3-458d-a0dc-310bf5908fcc.png align="center")

**3\. Git Tagging: Creating and Using Tags for Releases**

Tags in Git are used to mark specific points in history, often to signify release versions. To create a tag:

* Use the `git tag` command, followed by the tag name:
    

```bash
git tag v1.0
```

To tag a specific commit, specify the commit's SHA-1 hash:

```bash
git tag v1.1 abcdef1
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698289902180/491c0d4e-028a-4bb5-866b-ef5cf328f5bc.png align="center")

You can list all tags with `git tag`.

```bash
git tag
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698289967426/d0afb04a-fcae-42e5-9b60-40d085bc6c2f.png align="center")

**4\. Git Reset: Undoing Changes and Commits**

The `git reset` command is a powerful tool for undoing changes and commits in your project. It comes in three main modes: soft, mixed, and hard.

* **Soft Reset:** This mode moves the branch pointer without affecting your working directory or staging area. It's useful for uncommitting a commit.
    
* **Mixed Reset:** This mode moves the branch pointer and clears the staging area but retains your changes in the working directory.
    
* **Hard Reset:** This mode moves the branch pointer, clears the staging area, and discards all changes in the working directory.
    

For example, to undo the last commit and keep the changes in your working directory, use:

```bash
git reset --soft HEAD~1
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698290095579/7cc752a3-40ac-47fd-b8e0-921631c5f5f2.png align="center")

**5\. Git Ignore: Ignoring Files and Directories in Git**

The `.gitignore` file is used to specify files and directories that Git should ignore. This is particularly useful for excluding generated files, build artifacts, and sensitive data from version control. Create a `.gitignore` file in your project's root directory and list the patterns of files and directories you want to ignore.

For example, to ignore all files with the `.log` extension, your `.gitignore` file might contain:

```bash
*.log
```

**Conclusion**

Git's advanced techniques, including rebasing, commit history, tagging, resetting, and ignoring files, offer a deeper level of control and organization for your projects. By mastering these features, you can maintain a cleaner commit history, manage releases more efficiently, and navigate the complexities of version control with confidence. These techniques are invaluable for developers seeking to streamline their workflows and improve collaboration within their teams.