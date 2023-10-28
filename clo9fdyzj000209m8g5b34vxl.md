---
title: "Lecture7 # Enhancing Git Proficiency: Stash, Reflog, and Aliases"
datePublished: Sat Oct 28 2023 02:31:03 GMT+0000 (Coordinated Universal Time)
cuid: clo9fdyzj000209m8g5b34vxl
slug: lecture7-enhancing-git-proficiency-stash-reflog-and-aliases
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1698459588282/67316e61-aecb-4833-aa83-2120007b8d30.png
tags: github, git, devops, devops-articles, masterwithhamza

---

Git, a robust version control system, provides a multitude of features that extend beyond basic version tracking. In this article, we will delve into three advanced Git features: Git stash, Git reflog, and Git aliases. These tools are indispensable for managing work in progress, recovering lost commits, and customizing your Git workflow for efficiency.

### **1\. Git Stash: Saving and Applying Work in Progress**

Git stash is a versatile feature designed to help you manage changes in progress, allowing you to switch tasks or branches without committing to unfinished work. Here's how to leverage Git stash effectively:

**Stashing Changes:** When you want to set aside your current changes, use the command `git stash` without any arguments:

```bash
git stash
```

This command saves your changes to a new stash and reverts your working directory to a clean state.

**Listing Stashes:** You can view your stashes by running the `git stash list`. This command provides a list of your stashes, each with a unique name and timestamp.

```bash
git stash list
```

**Applying a Stash:** To apply a stash, use `git stash apply` followed by the stash name:

```bash
git stash apply stash@{1}
```

**Popping a Stash:** If you want to both apply and remove a stash in one go, you can use `git stash pop`.

```bash
git stash pop
```

**Clearing Stashes:** To remove a stash, use the `git stash drop` followed by the stash name.

```bash
git stash drop
```

Git stash allows you to manage ongoing work effectively, switch tasks seamlessly, and return to your work later without committing unfinished changes.

### **2\. Git Reflog: Recovering Lost Commits**

Git reflog is a crucial safety net that keeps track of actions on your branches, making it an invaluable tool for recovering lost commits or branches. Here's how to utilize Git reflog:

Git reflog is a crucial safety net that keeps track of actions on your branches, making it an invaluable tool for recovering lost commits or branches. Here's how to utilize Git reflog:

* **Viewing the Reflog:** To see the reflog, run `git reflog`. It displays a chronological list of recent actions on branches and their corresponding commit hashes.
    

```bash
git reflog
```

* **Recovering Lost Commits:** Locate the commit in the reflog that you want to recover, and then use `git branch branch-name commit-hash` to create a new branch at the desired commit.
    

```bash
git branch branch-name commit-hash
```

* **Restoring Deleted Branches:** If you accidentally delete a branch, the reflog can help you recover it. Use `git branch branch-name commit-hash` to recreate the branch.
    

```bash
git branch branch-name commit-hash
```

* **Undoing Mistaken Commits:** If you accidentally amend a commit, you can use `git reflog` to find the previous commit's SHA and reset your branch to that commit.
    

```bash
git reflog
```

Git reflog is a powerful tool for safely recovering lost commits and branches, providing confidence in managing your Git history.

### **3\. Git Aliases: Creating Custom Git Commands**

Git aliases enable you to create custom shorthand commands to streamline your Git workflow, save time, and reduce the risk of errors. Here's how to set up Git aliases:

* **Setting Up Aliases:** Open your Git configuration file with `git config --global --edit`. You can add your aliases like this:
    

```bash
[alias]
    co = checkout
    br = branch
    ci = commit
    st = status
    last = log -1 HEAD
```

* **Using Aliases:** Once you've defined aliases in your configuration, you can use them as if they were regular Git commands. For example, you can use `git co` instead of `git checkout`.
    
* **Advanced Aliases:** You can create more complex aliases that combine multiple Git commands into one. This can help automate repetitive tasks and make your workflow more efficient.
    

Git aliases offer an opportunity to tailor your Git workflow to your preferences, reducing typing and simplifying command execution.

### **Conclusion**

Git stash, Git reflog, and Git aliases are advanced features that can significantly enhance your Git experience. Git stash provides a structured way to manage ongoing work, Git reflog acts as a safety net for recovering lost commits and branches, and Git aliases allow you to create custom Git commands, simplifying your workflow and saving time. Incorporating these features into your daily Git routine can make you a more efficient and effective developer, further enhancing your Git proficiency.