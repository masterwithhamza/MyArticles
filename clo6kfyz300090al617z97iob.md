---
title: "Lecture3 # Git Essentials: Staging, Committing, Branching, Merging, and Resolving Conflicts"
datePublished: Thu Oct 26 2023 02:29:16 GMT+0000 (Coordinated Universal Time)
cuid: clo6kfyz300090al617z97iob
slug: lecture3-git-essentials-staging-committing-branching-merging-and-resolving-conflicts
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1698285794057/218ce9a0-47b6-4130-81db-fb0d0ecb8d4a.png
tags: github, git, devops, devops-articles, masterwithhamza

---

Git offers a powerful set of features to manage your project's version control effectively. In this article, we will delve into key Git concepts, including staging, committing, branching, merging, and resolving conflicts.

### **1\. Git Staging: Adding Changes to the Staging Area**

Staging is the process of selecting and preparing changes you want to include in your next commit. To stage changes:

* Use the `git add` command to specify which files or changes you want to include in the commit.
    

```bash
git add filename.ext
```

For example, to stage a specific file, run:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698286030079/120730f6-352c-4665-91df-c67576a9a5a2.png align="center")

* To stage all changes, use `git add .`
    

```bash
git add .
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698284457844/76b55933-c26e-4ccf-91fa-5d6e31ee73c8.png?auto=compress,format&format=webp align="left")

**2\. Git Commit: Creating a Commit with Staged Changes**

After staging changes, you can create a commit to record these changes in your project's history. A commit is like a snapshot of your project at a specific point in time. To commit staged changes:

* Use the `git commit` command, along with a meaningful commit message:
    

```bash
git commit -m "commited by hamza rehman"
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698284650258/baae94d5-bd53-4fc3-a891-02a935854520.png?auto=compress,format&format=webp align="left")

This creates a commit with the staged changes and a descriptive message.

**3\. Git Branches: Creating and Managing Branches**

Branches in Git allow you to work on different features or fixes independently, keeping your main codebase clean. To create and manage branches:

* To create a new branch, use the `git branch` command:
    

```bash
git branch hamza
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698286412641/c11ef1c1-f774-4b33-bf41-1c9fe89f904e.png align="center")

To switch to a branch, use the `git checkout` command:

```bash
git checkout hamza
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698286502652/bc67765f-3d16-4369-aa81-6d06837b56b6.png align="center")

To create and switch to a new branch in one command, you can use `git checkout -b`:

```bash
git checkout -b rehman
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698286629240/346952bd-ceb2-4887-9754-905fa6a57bb2.png align="center")

* To list all branches, use `git branch`.
    
    ```bash
    git branch
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698286681379/6d10a4c5-cc99-4451-923d-45c3930117b4.png align="center")
    
    To delete a branch, use `git branch -d branch-name`
    

```bash
git branch -d rehman
```

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698286799334/44dfa7f3-638d-4d32-97ea-73543114a2d6.png align="center")

**4\. Merging Branches: Combining Changes from One Branch into Another**

Merging is the process of combining changes from one branch into another. Typically, you merge feature branches into the main branch to incorporate new functionality or bug fixes. To merge branches:

* Ensure you are on the branch where you want to merge changes (e.g., the main branch).
    
* Use the `git merge` command, followed by the branch you want to merge:
    

```bash
git merge rehman
```

This combines the changes from `rehman` into your current branch.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698287021627/8a9587d7-4585-49a4-b92e-371ad77cebf9.png align="center")

**5\. Resolving Conflicts: Dealing with Merge Conflicts**

In collaborative projects, merge conflicts can occur when two branches have conflicting changes. Git cannot automatically determine which changes to keep. To resolve conflicts:

* Git will notify you of the conflict when you attempt to merge.
    
* Open the conflicted file in a text editor.
    
* Manually resolve the conflict by choosing which changes to keep.
    
* Remove conflict markers (e.g., `<<<<<<<`, `=======`, `>>>>>>>`) from the file.
    
* Save the file.
    
* Stage the resolved file using `git add`.
    
* Commit the resolution with a descriptive message using `git commit`.
    

**Conclusion**

Understanding Git's core concepts, including staging, committing, branching, merging, and conflict resolution, is essential for effective version control. By mastering these skills, you can manage your project's development efficiently, collaborate with others seamlessly, and maintain a well-organized codebase. Git's versatility and reliability make it a vital tool for software developers and teams.