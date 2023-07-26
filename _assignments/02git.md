---
title: "Week 2: Git"
layout: single
author_profile: false
classes: wide
excerpt: Practice git skills
---

## Initializing a new repository:
1. Create an empty folder called `new_project` in a sensible location on your computer. 
2. Initialize the folder as a git repository.  
    * *Remember that every project should be its own git repository.*
    * *Do NOT initialize root directories or parent folders relating to different projects*
3. Verify that the .git folder is now in the directory.

## Make your first commit
1. Check the git status 
2. Create a new file called `file_1.txt` 
3. Create another new file called `file_2.txt` 
4. Check the git status 
5. Add both files to the staging area
6. Check the git status
7. Commit the new files using the commit message "create new files"
8. Check the git status 
9. Check the git log 

## More git practice
 1. Open `file_1.txt` in a text editor.   Add the following to the file:
    ```
    This is my first file.
    ```
2. Open the the `file_2.txt` in a text editor.  Add the following to the file: 
    ```
    This is my second file.
    ```
3. Save the changes to both file.  Check the git status
4. Add and commit only the changes from the `file_1.txt` file.  Check the git status.
5. Make another commit with only the changes from the `file_2.txt` file.
6. Check the git log

## Readme file
Even more committing practic    - (a) In the text editor, make more changes to both the `statistics.txt` and the `history.txt` files. For example, add a few more curriculum ideas. Save your changes.  
    - (b) Add and commit the new changes.  This can be done however you want.  For example:  add all the changes to staging then commit.  Or, add and commit all the changes in one step.    

## .gitignore
7. Ignore files
    - (a) Create a .gitignore file with the following text "api-keys.txt" 
    - (b) Add and commit the .gitignore file
    - (c) Create a file called "api-keys.txt" 
    - (d) Check the status of the git repo

## Working with branches
8. Branches
    - (a) Make new branch called "music"
    - (b) Switch to the "music" branch
    - (c) Look at the log
    - (d) Create a new file called `music.txt`
    - (e) Add and commit the new file with the commit message "add empty music file"
    - (f) Add some curriculum topic ideas to the `music.txt` file
    - (g) Commit the changes to the current branch
    - (h) Make another new branch off of the music branch HEAD called "orchestra"
    - (i) Switch to the new branch
    - (j) Create a new file (called whatever you want) and put some text in it
    - (k) Save, add, and commit
    - (l) Merge the orchestra branch into the music branch and then delete the orchestra branch
    - (m) Check logs and statuses along the way
    - (n) Merge all the changes into the main branch and then delete the music branch
 
## Practice with remote repositories 
10. Push repository to GitHub
    - (a) Create a blank repository in your GitHub account called "CourseDevelopmentIdeas.  Do not initialize it with a readme file or a .gitignore file.
    - (b) Copy the SSH url.
    - (c) On your local machine, set the remote branch by typing `git remote add origin <ssh url>`
    - (d) Push the local repo up to GitHub by typing `git push -u origin main`
    - (e) Check that your GitHub repo was updated with your local work
11. Save a file with your git commands
    - (a) In the terminal type `history | grep "git " > git_commands.txt` (or if using a zsh terminal type `history 0 | grep "git" > git_commands.txt`)
    - (b) You should now have a file called "git_commands.txt". Submit this file as part of homework 1

## Merge conflicts

## GitHub Pages

