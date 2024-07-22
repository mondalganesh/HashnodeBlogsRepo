---
title: "How to start with git! using Visual Studio Code?"
seoTitle: "Start with Git in Visual Studio Code"
seoDescription: "Learn how to set up and use Git with Visual Studio Code for version control and project management"
datePublished: Mon Jul 22 2024 03:40:53 GMT+0000 (Coordinated Universal Time)
cuid: clywfw23s000709laeui3853t
slug: how-to-start-with-git-using-visual-studio-code
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1721585969633/9a2f3e94-4869-4830-8776-8b7e6c036310.png
tags: github, opensource, devops, contribution-to-open-source, devops-learning

---

**I am assuming Git and VS Code are already installed on your system.**

1. **Open VS Code**
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1721577279910/7be61b8e-68d2-4f85-b29e-86ab19ef3c7f.png align="left")
    
2. **Navigating the Git Repository**
    

To create a fresh new project, go to Files and select **Open Folder**.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1721572488358/51b02950-fd11-4920-a285-1001cefc564e.png align="left")

Select the folder where you want to store your projects/repositories. This folder will be called your present work directory.

3. Right-click and open the Integrated Terminal.
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1721574945010/87e6c341-e52e-4390-8813-7aad93b796aa.png align="left")

4. Check the Git version installed on your system and verify the installation:
    

```plaintext
git --version
```

If the installed Git version on your system is old and you want to update it, you can skip this step if you have done a fresh installation:

```plaintext
git update
```

5. **Configure Your Git**
    

**Why do you need to configure your Git?**

It is very important to configure your Git locally with basic details like username and email address so that when you contribute to any of your open-source or office projects, anyone can easily understand who has contributed to that particular assignment/task.

**How to check what details are configured?**

```plaintext
git config --list
```

```plaintext
git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"
```

Another way, if you have already set up your configuration file in Git, you can open and edit the file. You can skip this step if you have done a fresh installation. 🛠️

```plaintext
git config --global --edit
```

a) Now you are inside the "Vi editor/terminal". Use insert mode and make the changes in the configuration file.

Press 'i' to enable editing:

b) Enter or modify the user details:

For example:

```plaintext
user.name = Ganesh Mondal
user.email = ganeshm@abc.com
```

c) To save the details, press **Esc**, then type `:wq`. It will save and quit the terminal.

d) Verify the configurations by listing existing configurations:

```plaintext
git config --list
```

***Main task is done. Now, we will create our first version for Git code.***

6. **Understand the Flow of Git**
    

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1721584925602/19414c49-0b8e-45a0-838a-806c5ba56b6c.png align="center")

a) **Work Directory**: Where your files and code are stored on the local machine.

b) **Staging Area**: Where the files and code are staged after `git add`. You can still revert your changes as they are not yet committed. The staging area is denoted with green color.

c) **Local Repository**: After commit, code/files are now versioned. Commit changes cannot be reverted. If really needed, you can go back to a previous version.

d) **Remote Repository**: This area is a remote server, such as GitHub, GitLab, etc. For code collaboration. The remote repository is important as sharing and making the code public/private will be easy. Others can clone and fork the repository to contribute to enhancing the code functionality.

When any repository is added from local to remote, it is known as a Push request. Similarly, if anyone contributes any functionality to your code, that person needs to send a Pull request so that the project owner can verify the changes and accept/reject the contribution.

7. **Initialize the Repository**
    

Always initialize the folder/directory. Once initialized, Git versioning will start after that.

```plaintext
git init
```

A `.git` hidden directory will be created in your selected folder. Never delete any files from there; else, it will result in corrupting your Git repository's version history.

8. **Add Files to the Staging Area**
    

* `.` - Denotes all the files and folders in the present directory.
    
* `<filename>` - If only one file needs to be staged, then provide that file name.
    
* `*` - Denotes all the files, a wildcard character.
    

```plaintext
git add .
```

or

```plaintext
git add <filename>
```

or

```plaintext
git add *
```

9. **Commit the Changes to Create a Version ✍️**
    

`-m` - Denotes the message to the commit.

The `git commit` command will automatically pick the latest staged files in green:

```plaintext
git commit -m "Initial commit"
```

10. **Check the Status of Your Repository**
    

```plaintext
git status
```

11. **Check Logs of Your Commit for All the Versions**
    

```plaintext
git log
```

or

```plaintext
git log --oneline
```

Wonderful! You have successfully made your first commit to Git. Learn with simplicity.

## **What Coming Next**

In the upcoming blogs,

* We will disscuss more on "impact of Git on an Open source projects".
    
* Why students should adopt this tool early from college days?
    
* How a Git can be useful in crowd sourcing?
    
* We will start an open-source mini project for all students to contribute.
    
* and much more to explore...
    

---

Hope you find this blog informative and helpful. If you have any questions or need further assistance with Git, feel free to drop a comment below! Happy coding! 💻😊

---

***This Blog is sponsored by*** [**KhojiLabs.com**](https://khojilabs.com)***. Khoji Labs provides all the necessary free guidance to college students to help them grow in their careers.***

---