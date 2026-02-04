# Git Cheat sheet

Okay first thing you need to know is git is divided into like sections like a tree

First you have your repositories

- Local repository (you make this using *git init)*
- Remote repository (what you have on github)

The local repository is divided to

1. Working directory (The place you have your files on just the regular windows folder)
2. Staging area (I’ll explain this later bit confusing)
3. Repository (this is like a hidden folder where the stuff you commit to will go to. This is what gets uploaded to github)

 

[![image.png](https://miro.medium.com/v2/resize:fit:1100/format:webp/1*diRLm1S5hkVoh5qeArND0Q.png)

## Local Repository

### Working directory

Like I said this is the place you would see on your file explorer or vscode navigation bar.  Let’s say you made a change to an html file and ctr+c it or created a new python this is the place it’ll go to without doing any git commands. Then comes the staging area.

### Staging area

The commands related to this part are:

- *git add .* - the dot signifies that you’re adding all the files in the working directory to the staging area even if you have changed them or not. New and deleted files would be added asw
- git add <file name> - when you want to add a specific file only to the staging area. Ex: index.html would be *git add index.html.* you can run this multiple times for different files before committing.
- git add -A - This would only add files that have **changed/modified, deleted, or new files** since the last commit **.**

This is like the place you are using to pick which files to commit aka save to the local repo.

Let’s say you accidently added a file you don’t want to commit rn to the stagin area, then you’ll have to run this command

*git restore --staged <file name>*

### Repository

This is like a hidden save file
