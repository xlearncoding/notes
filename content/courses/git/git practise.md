---
title: git practise
---

In this section of mini course git, I will cover the very basics of Git. I will start by creating a folder and initializing Git in it. Next, I will create a text file with "Hello World" text inside it. I will then commit this file to Git and view it in the commit log. Finally, I will revert back to a previous commit to demonstrate how Git can track changes throughout the journey. This section will provide a practical introduction to Git and its fundamental functionalities.

## Step 1: Create a folder

[[open your terminal|Open your terminal]] or [[open your Command Prompt|command prompt]], navigate to the directory where you want to create your mini Git course folder, and then run the following command to create a new folder:

```bash
mkdir git-test
```


## Step 2: Navigate into the folder

Run the following command to navigate into the folder you just created:

```bash
cd git-test
```

Now run the `ls -lah` command to list and see the files and directories in this folder. Confirm the folder is empty for now.


## Step 3: Initialize a Git repository

Run the following command to initialize a new Git repository in the folder:

```bash
git init
```

Now run again the `ls -lah` command and see the `.git` folder created with the `git init` command. All your commit history and changes will be held in this hidden `.git` folder.

<iframe width="560" height="315" src="https://www.youtube.com/embed/6OOFo0Nh_SA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Step 4: Create a text file with "Hello World" text

Run the following command to create a new text file called `hello.txt` with "Hello World" text in it:

```bash
echo "Hello World" > hello.txt
```

* You can also use [[Vim text editor]] to create this file and include "Hello World" text in it as I am doing in the below video.

You can check the text in `hello.txt` file with this command:

```bash
cat hello.txt
```

Or simply open the file and read the text.

## Step 5: Add and commit the text file

Now run this command to see you have git unstaged changes:

```bash
git status
```

The filename `hello.txt` is listed in the output with red color. The red color indicates that you haven't added your changes to git yet. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/CHC_87kWLGM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

Now run the following commands to add the `hello.txt` file to the Git repository:

```bash
git add hello.txt
```

Now run the `git status` command again and you will see the filename is in green. Now run the following command to commit your changes and add it to the new version of your repository:

```bash
git commit -m "Added hello.txt with Hello World text"
```

The `-m` argument in Git allows you to add a commit message that serves as a reminder of the changes you made. This commit message is essential for keeping track of your changes in the future when you review the commit logs. It's a good practice to provide a meaningful and descriptive commit message that accurately reflects the changes made in the commit. This will help you and your collaborators easily understand the purpose and content of the commit when looking back at the commit history.

## Step 6: Show the commit in the log 

Run the following command to show the commit you just made in the Git log:

```bash
git log
```

You should see the commit message and other details of the commit in the log.

<iframe width="560" height="315" src="https://www.youtube.com/embed/-9U9FYyDcIc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## Step 7: Revert back to the initial state

Now, let's revert back to the initial state where there was no `hello.txt` file. Run the following command to revert the last commit:

```bash
git revert HEAD
```

This will create a new commit that undoes the changes made in the previous commit, effectively reverting back to the initial state.

## Step 8: Show the revert commit in the log

Run the following command to show the revert commit in the Git log:

```bash
git log
```

You should be able to observe the details of the revert commit, including the commit message and other relevant information, in the Git log. This showcases the powerful tracking capabilities of Git, which is a key aspect covered in this section of the mini course git. The ability to view and understand the changes made to your codebase through the commit log is an essential skill in effective version control, allowing you to effectively manage and track the history of your project.

<iframe width="560" height="315" src="https://www.youtube.com/embed/TzUtIy0cg2Q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## Final note

As you conclude this last section, you now have a solid understanding of the basics of Git and version control. Git is a powerful tool that allows you to track changes, collaborate with others, and manage your codebase efficiently. With Git, you can easily revert to previous versions, compare changes, and manage multiple branches of your codebase. It's a crucial skill for any software developer, as version control is a fundamental aspect of modern software development workflows.

By mastering the basics of Git, you have taken a significant step towards becoming a more proficient developer. With continued practice and experience, you can leverage the full power of Git to streamline your development process, collaborate effectively with others, and efficiently manage your codebase. Keep experimenting with Git and incorporating it into your workflow to enhance your coding capabilities.

Congratulations on your progress so far! You now have a solid foundation in Git and version control. Keep exploring and experimenting with Git, and you'll be well on your way to becoming a proficient Git user. Great job! Keep up the good work, and remember, practice makes perfect.

Happy coding!
