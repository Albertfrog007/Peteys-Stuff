# Introduction to Git

[

1. Setup instructions



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#d5e9c2b6379246a593c1ef74051e7e3c)

[

Configuring Your Name & Email



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#3f395b09dee24f738fea3ee6f14ed220)

[

2. Repositories



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#5b7377e4b75a4a32bfe992c47b3697e7)

[

3. Initializing a repository



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#bbd762b064204f88aefafe7860c6d424)

[

4. Staging and committing code



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#7f511618e855423c935dc05ade74b3b6)

[

4.1. Checking the status



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#3c2d44215f924a1e8e18a9877e13d5da)

[

4.2. Staging files



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#8ef167b4285649fb9de21e4bb4114d66)

[

4.3. Making commits



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#3d067e361bbf48d18d7b543421fc2923)

[

4.4. Commit history



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#3b2cb3502d4e4eadb067055cc170220b)

[

4.5. Ignoring files



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#90547dd920ae47bb987c6e2b40f880e7)

[

5. Branches



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#a2aa5d735af844e6909e0918cf3110c5)

[

5.1. Creating a new branch



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#e0920693bebe4ffd94e973d60bd3f6b4)

[

5.2. Changing branches



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#ed1c8d1fb07d4f46b1cf05730c0c2b7c)

[

5.3. Merging branches



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#5d881566c7e74a58830f944eacd57d3e)

[

5.4. Deleting a branch



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#1a887888322b44168d8976ebfde7fcc2)

[

6. Further learning



](https://zarkom.notion.site/zarkom/Introduction-to-Git-ac396a0697704709a12b6a0e545db049?pvs=25#9e4f2808a75643a58fa45932ea7f38a1)

Git is officially defined as a distributed version control system (VCS).

In other words, it's a system that tracks changes to our project files over time. It enables us to record project changes and go back to a specific version of the tracked files, at any given point in time. This system can be used by many people to efficiently work together and collaborate on team projects, where each developer can have their own version of the project, distributed on their computer. Later on, these individual versions of the project can be merged and adapted into the main version of the project.

Basically, it's a massively popular tool for coordinating parallel work and managing projects among individuals and teams. Needless to say, knowing how to use Git is one of the most important skills for any developer nowadays - and it's definitely a great addition to your resume!

![ℹ️](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

Git official homepage: [https://git-scm.com/](https://git-scm.com/)

## 1. Setup instructions

Git is primarily used via the command-line interface, which we can access with our system terminals.

However, we first need to make sure that we have Git installed on our computers.

![ℹ️](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

You can download Git here: [https://git-scm.com/downloads](https://git-scm.com/downloads)

Click the download link for your specific operating system and then follow through the installation wizard to get things set up on your computer!

After installing it, start your terminal and type the following command to verify that Git is ready to be used on your computer:

Bash

git --version

​

If everything went well, it should return the Git version that is installed on your computer.

![Callout icon](https://zarkom.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F094d32ef-20c1-421d-944b-200ec14f150b%2Fapple.png?table=block&id=248844c1-09f1-456b-a6ae-51408a7b2fe9&spaceId=998f501b-5134-4b2d-bdc1-d18e03f19f76&width=40&userId=&cache=v2)

If you are using a Mac or Linux machine, then you can utilize the default Bash terminal that comes pre-installed on your machine.

![Callout icon](https://zarkom.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F32663572-2b24-4079-bf3f-29f2146d2b56%2Fwindows.ico?table=block&id=62f52b51-0b91-48fd-a238-84bcde16f5cc&spaceId=998f501b-5134-4b2d-bdc1-d18e03f19f76&userId=&cache=v2)

If you are using Windows, you can use its built-in Powershell terminal, or the Git Bash terminal which is bundled with the Git installation. For detailed windows Git and Git Bash install instructions, check out this blog post: [https://zarkom.net/blogs/how-to-install-git-and-git-bash-on-windows-9140](https://zarkom.net/blogs/how-to-install-git-and-git-bash-on-windows-9140)

#### Configuring Your Name & Email

In your terminal, run the following commands to identify yourself with Git:

Bash

git config --global user.name "Your Name" git config --global user.email "your@email.com"

​

Replace the values inside the quotes with your name and email address.

## 2. Repositories

When working with Git, it's important to be familiar with the term repository. A Git repository is a container for a project that is tracked by Git.

We can single out two major types of Git repositories:

Local repository - an isolated repository stored on your own computer, where you can work on the local version of your project.

Remote repository - generally stored outside of your isolated local system, usually on a remote server. It's especially useful when working in teams - this is the place where you can share your project code, see other people's code and integrate it into your local version of the project, and also push your changes to the remote repository.

In this video, we'll only work with local repositories.

## 3. Initializing a repository

To create a new repository and start tracking your project with Git, use your terminal software and navigate to the main folder of your project, then type the following command:

Bash

git init

​

This command will generate a hidden .git directory for your project, where Git stores all internal tracking data for the current repository.

## 4. Staging and committing code

Committing is the process in which the changes are 'officially' added to the Git repository.

In Git, we can consider commits to be checkpoints, or snapshots of your project at its current state. In other words, we basically save the current version of our code in a commit. We can create as many commits as we need in the commit history, and we can go back and forth between commits to see the different revisions of our project code. That allows us to efficiently manage our progress and track the project as it gets developed.

Commits are usually created at logical points as we develop our project, usually after adding in specific contents, features or modifications (like new functionalities or bug fixes, for example).

![📌](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

Before we can commit our code, we need to place it inside the staging area.

### 4.1. Checking the status

While located inside the project folder in our terminal, we can type the following command to check the status of our repository:

Bash

git status

​

This is a command that is very often used when working with Git. It shows us which files have been changed, which files are tracked, etc.

We can add the untracked project files to the staging area based on the information from the git status command.

At a later point, git status will report any modifications that we made to our tracked files before we decide to add them to the staging area again.

### 4.2. Staging files

From the project folder, we can use the git add command to add our files to the staging area, which allows them to be tracked.

We can add a specific file to the staging area with the following command:

Bash

git add file.js

​

To add multiple files, we can do this:

Bash

git add file.js file2.js file3.js

​

Instead of having to add the files individually, we can also add all the files inside the project folder to the staging area:

Bash

git add .

​

By default, this adds all the files and folders inside the project folder to the staging area, from where they are ready to be committed and tracked.

### 4.3. Making commits

A commit is a snapshot of our code at a particular time, which we are saving to the commit history of our repository. After adding all the files that we want to track to the staging area with the `git add` command, we are ready to make a commit.

To commit the files from the staging area, we use the following command:

Bash

git commit -m "Commit message"

​

Inside the quotes, we should write a commit message which is used to identify it in the commit history.

The commit message should be a descriptive summary of the changes that you are committing to the repository.

After executing that command, you will get the technical details about the commit printed in the terminal. And that's basically it, you have successfully made a commit in your project!

![📌](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

To create a new commit, you will need to repeat the process of adding files to the staging area and then committing them after. Again, it's very useful to use the git status command to see which files were modified, staged, or untracked.

### 4.4. Commit history

To see all the commits that were made for our project, you can use the following command:

Bash

git log

​

The logs will show details for each commit, like the author name, the generated hash for the commit, date and time of the commit, and the commit message that we provided.

To go back to a previous state of your project code that you committed, you can use the following command:

Bash

git checkout <commit-hash>

​

Replace <commit-hash> with the actual hash for the specific commit that you want to visit, which is listed with the git log command.

To go back to the latest commit (the newest version of our project code), you can type this command:

Bash

git checkout master

​

### 4.5. Ignoring files

To ignore files that you don't want to be tracked or added to the staging area, you can create a file called .gitignore in your main project folder.

Inside of that file, you can list all the file and folder names that you definitely do not want to track (each ignored file and folder should go to a new line inside the .gitignore file).

You can read an article about ignoring files [on this link](https://help.github.com/en/articles/ignoring-files).

## 5. Branches

A branch could be interpreted as an individual timeline of our project commits.

With Git, we can create many of these alternative environments (i.e. we can create different branches) so other versions of our project code can exist and be tracked in parallel.

That allows us to add new (experimental, unfinished, and potentially buggy) features in separate branches, without touching the 'official' stable version of our project code (which is usually kept on the master branch).

When we initialize a repository and start making commits, they are saved to the master branch by default.

### 5.1. Creating a new branch

You can create a new branch using the following command:

Bash

git branch <new-branch-name>

​

The new branch that gets created will be the reference to the current state of your repository.

![📌](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

It's a good idea to create a development branch where you can work on improving your code, adding new experimental features, and similar. After development and testing these new features to make sure they don't have any bugs and that they can be used, you can merge them to the master branch.

### 5.2. Changing branches

To switch to a different branch, you use the git checkout command:

Bash

git checkout <branch-name>

​

With that, you switch to a different isolated timeline of your project by changing branches.

![📌](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

For example, you could be working on different features in your code and have a separate branch for each feature. When you switch to a branch, you can commit code changes which only affect that particular branch. Then, you can switch to another branch to work on a different feature, which won't be affected by the changes and commits made from the previous branch.

To create a new branch and change to it at the same time, you can use the -b flag:

Bash

git checkout -b <new-branch-name>

​

![ℹ️](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

To list the branches for your project, use this command: git branch

To go back to the master branch, use this command:

Bash

git checkout master

​

### 5.3. Merging branches

You can merge branches in situations where you want to implement the code changes that you made in an individual branch to a different branch.

For example, after you fully implemented and tested a new feature in your code, you would want to merge those changes to the stable branch of your project (which is usually the default master branch).

To merge the changes from a different branch into your current branch, you can use this command:

Bash

git merge <branch-name>

​

You would replace <branch-name> with the branch that you want to integrate into your current branch.

### 5.4. Deleting a branch

To delete a branch, you can run the git branch command with the -d flag:

Bash

git branch -d <branch-name>

​

![ℹ️](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

Read more about branching and merging [on this link](https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging).

## 6. Further learning

To learn more about Git, make sure to check the following resources:

Git official documentation: [https://git-scm.com/doc](https://git-scm.com/doc)

The free Pro Git book: [https://git-scm.com/book/en/v2](https://git-scm.com/book/en/v2)

Learn about GitHub: [https://guides.github.com/](https://guides.github.com/)

![ℹ️](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

GitHub is a website where we can store our repositories online. In other words, GitHub works with Git as a repository hosting service.