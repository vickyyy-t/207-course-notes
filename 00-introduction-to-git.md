# Chapter 0: Introduction to Git

## 0.1. What is Version Control?
- a way for us to control the versions of our code.
- tracking the changes that we've made, and control our revisions.

## 0.2. How version control works
In version control systems, there is a **master** repository: a copy of the latest versions of all files. People **clone** the repository to get their own local copy, which they work on independently.

As people make changes and reach a state that they want reflected in the master repository, they **push** their changes in. Similarly, anyone who wants the latest version of the repository will **pull** the changes.

## 0.3. Git
In git, the master repository is also known as the **origin**.

- `git status`: Lets us see what files have changed in our local copy
- `git clone <url>`: Get a local copy of the repository
- `git add <files>`: Lets us add ("stage") files that we want to modify in the origin
- `git commit -m "<message>"`: Saves our changes to the local repository, labelling the added changes with a message to describe our changes
- `git push`: Pushes changes to the origin repository
- `git pull`: Copy over any changes into your local repository

### 0.3.1. Branches
make a new **branch**: this is a spinoff of the master repository, in which you can commit changes without worrying about the master branch until you're ready to merge it in.
- `git checkout -b <branch name>`: creates a new branch, and switches your local repository to the new branch
- `git checkout <branch>`: change local repository to that branch

when ready to merge your branch into the master repository:
- checkout your master branch
- `git merge <branch name>` (nicer method is to make a pull request)