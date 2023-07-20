---
title: "Week 2: Git"
layout: single
author_profile: false
classes: wide
excerpt: Practice git skills
---

Initializing a new repository:
1. Create an empty folder called "NewProject" in a sensible location on your computer. 
2. Initialize the folder as a git repository.  
3. Verify that the .git folder is now in the directory.

Make 
4. Create a file called data ***.txt

1. Check which version of git is installed on your computer
2. Configure git 
    - (a) If you haven't already done so, configure git on your computer with your name, email, and text editor of choice.
    Change the default branch to "main." 

3. Create a git repo 
    - (a) Create a new folder called "CourseDevelopment" 
    - (b) Navigate to the new folder in the terminal 
    - (c) Initialize the folder to be a git repository 
    - (d) Verify that the .git folder is now in the directory 
4. Make first commit
    - (a) Check the git status 
    - (b) Create a new file called `statistics.txt` 
    - (c) Create another new file called `history.txt` 
    - (d) Check the git status 
    - (e) Commit the new files using the commit message "create course outline files" 
    - (f) Check the git status again 
5. More committing practice
    - (a) Open the `statistics.txt` in a text editor.   Add the following to the file:
    ```
    Ideas for curriculum: 
    
        - Mean and standard deviation
        - Regression
        - Bayes Theorm
    ```
    - (b) Open the the `history.txt` in a text editor.  Add the following to the file: 
    ```
    Ideas for curriculum:
    
        - Roaring Twenties
        - The Great Depression
        - World War II
    ```
    - (c) Be sure to save the changes before moving on
    - (d) Commit only the changes from the `statistics.txt` file.  Use the message "add statistics curriculum ideas" 
    - (e) Make another commit with only the changes from the `history.txt` file. Use the message "add history curriculum ideas" 
6. Even more committing practice
    - (a) In the text editor, make more changes to both the `statistics.txt` and the `history.txt` files. For example, add a few more curriculum ideas. Save your changes.  
    - (b) Add and commit the new changes.  This can be done however you want.  For example:  add all the changes to staging then commit.  Or, add and commit all the changes in one step.    
7. Ignore files
    - (a) Create a .gitignore file with the following text "api-keys.txt" 
    - (b) Add and commit the .gitignore file
    - (c) Create a file called "api-keys.txt" 
    - (d) Check the status of the git repo
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
9. GitHub and SSH
    - (a) Sign up for a GitHub account if you haven't already done so
    - (b) Follow the instructions [here](https://docs.github.com/en/authentication/connecting-to-github-with-ssh) to connect to GitHub with SSH.  For a brief summary of these instructions, see [this](https://stat426-fall2021.github.io/blog/ssh-and-github) blog post.  
10. Push repository to GitHub
    - (a) Create a blank repository in your GitHub account called "CourseDevelopmentIdeas.  Do not initialize it with a readme file or a .gitignore file.
    - (b) Copy the SSH url.
    - (c) On your local machine, set the remote branch by typing `git remote add origin <ssh url>`
    - (d) Push the local repo up to GitHub by typing `git push -u origin main`
    - (e) Check that your GitHub repo was updated with your local work
11. Save a file with your git commands
    - (a) In the terminal type `history | grep "git " > git_commands.txt` (or if using a zsh terminal type `history 0 | grep "git" > git_commands.txt`)
    - (b) You should now have a file called "git_commands.txt". Submit this file as part of homework 1

## Part 2: Setup your github profile
1. Add a picture
2. Add your name
3. Add a brief bio
4. Create a [profile README](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)

## Part 3: Create your blog

1. Clone the blog template onto your local machine
    - (a) In your terminal navigate to the local directory where you want to store your blog files
    - (b) Type `git clone git@github.com:esnt/my386blog.git`.  There should now be a new directory called "my386blog".
    - (c) Navigate inside the "my386blog" folder
2. Create a new repository in your GitHub account called "my386blog".  Do not initialize with a readme or .gitignore.
3. Link your local blog template to your GitHub repo
    - (a) Copy the ssh url of the my386blog repo from YOUR GitHub account
    - (b) On your local machine, be sure you are in the "my386blog" folder
    - (c) Change the remote path of the local blog by typing in your local terminal `git remote set-url origin <ssh-url>` 
4. Push the repo to GitHub
    - (a) Push the entire repository to GitHub by typing `git push -u origin main`
    - (b) Check on GitHub that the repo is now filled
5. Set up GitHub Pages
    - (a) In GitHub, go the repo settings
    - (b) On the left hand side, choose "Pages"
    - (c) Under "Build and Deploy", select "Deploy from Branch"
    - (d) Under "Branch", select the main (or master) branch and hit save
    - (e) It takes a few minutes for everything to get set up.
6. Make your blog url easy to access
    - In the main repo page, on the right hand side there is an "About" section.  Click on the gear symbol to edit.  Add the blog url to the website field (the blog url is most likely "https://your-username.github.io/my386blog"
7. Personalize your blog by editing the template.
   *You should make these change on your local machine and push the changes to GitHub* 
   
  > *NOTE: Occasionally it might be necessary for you to make changes directly in GitHub.  In this situation remember the following:* 
  > * Before you make any changes in GitHub:  run a `git push` locally to ensure that GitHub has the latest local changes
  > * Before you make any changes locally: run a `git pull` to ensure that your local repo has the latest GitHub changes

    - (a) Update the `_config.yml` file
        * Change the blog title
        * Change the email to your email
        * Change the description
        * Leave the baseurl as is (unless you called your repo something other than my386blog)
        * Change the url to `https://your-github-username.github.io`
        * Change the blog image .  New images should be put into the `assets/images` folder.  When I download from a source like unsplash, I usually use the "medium" size
        * Change the author to your name
        * Change the copyright to what you'd like it to be or leave empty
        * Change the social media tags to your own usernames.  Leave blank for any fields that you don't want displayed (You should at least have GitHub)
        * Save, add, commit (and push to GitHub if necessary)
    - (b) Edit the `about.markdown` file
        * Using markdown, add a description about you in the `about.markdown` file.  Do not edit the heading  (anything in between `---`)
    - (c) Make a new blog post just to practice
        * Follow the instructions in the sample blog post to make a new blog post called `2023-01-26-blog-ideas.md
        * Your blog post needs to have a heading.  Be sure that the "layout" is "post", but all other fields should correspond to your post
        * In the body of your blog post, include ideas that you have for your future blog posts:  
            - What are you planning on doing for your "how-to" post? 
            - What book are going planning on reading for data science ethics?  
            - Where are you hoping to get data for your main class project?  
        * Add an image to your post (both in the header and in the body of the post)
8. Activate comments on your blog.
Follow the instruction below to use "utterances" for your blog comments.  You are welcome to use other commenting tools (such as disqus) if you have experience, but I am only going to teach how to install and use utterances.  

    1. Intall the utterances app on in your blog repository  
        a. Go to [https://github.com/apps/utterances](https://github.com/apps/utterances)   
        b. Click "Configure"  
        c. Choose the repository where you want to install utterances (your blog repo). 
            * Select your user name. 
            * Select "Only select repositories". 
            * Choose your blog repository. 
            * Click install. 

    2. In your repository, go to settings and make sure that "Issues" are turned on.  You'll find "Issues" on the main settings page under "Features".  Check the box next to "Issues."

    3.  Navigate to the "\_layouts" folder and open "post.html" file. 

    Find the following code in the file:
    ```
    <script src="https://utteranc.es/client.js"
        repo="your-user-name/my386blog"
        issue-term="pathname"
        label="💬"
        theme="boxy-light"
        crossorigin="anonymous"
        async>
    </script>
     ```
    4. Change "your-user-name" in the second line in the code block to your actual github user name.  For example, in my blog the second line in the code block should be `repo="esnt/my386blog"`.  



## Part 4: Submitting your Homework
When you clicked on the link for this assignment in LearningSuite, you were asked to accept this homework assignment.  After you accepted the assignment,  GitHub Classroom created a private repository for you named "your-github-name-hw-01". 

    - GitHub Classroom sets up this repo with a homework template that I've provided 
    - It also creates permissions so that only you and the organization owners (me and the TA) have access to it 
    
In order to submit your homework, you need to add files to this repository:  
    (1). The "git_commands.txt" file that you created in part 1
    (2). Create a file called "myblog.txt" where the body of the file is just the url for your class blog.
    
> Note:  You can add files by direct upload through GitHub or by first cloning the repo locally, adding files locally, and pushing back to GitHub.  



