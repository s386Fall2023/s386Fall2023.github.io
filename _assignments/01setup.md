---
title: "Week 1: Getting set up"
layout: single
author_profile: false
classes: wide
excerpt: Get everything needed for class set up this week.
#header:
#   teaser: /assets/images/frog.png  
---
Objective:  Setup the tools that we'll be using this semester in Stat 386.

Instructions: Follow the direction below to get Git, GitHub, Anaconda, and VS Code up and running.

## Install necessary software

### 1. Git
1. Download and install [git](https://git-scm.com/) onto your computer (version should be 2.33 or greater)
    * Verify that the installation was successful:
        - On a mac: Open the terminal and type `git --version`.  It should return `git version X.XX.XX` (with the version number)
        - On a PC: Verify that you have "git bash".  Open "git bash" and type `git --version` to verify your version number.

2. Configure git 
    * Configure git on your computer with your name, email, and text editor of choice.
    * Change the default branch to "main" (instead of "master") 

---
### 2. Anaconda 
1. Download and install [anaconda](https://www.anaconda.com/download) or [miniconda](https://docs.conda.io/en/latest/miniconda.html) onto your computer
2. Create a virtual environment for our class:
    * In the terminal (Mac) or Anaconda promt (Windows) type
    ```conda create --name stat386 python==3.10```
    * Activate the environment you just created:
    ```conda activate stat386```
    * Conda install the packages we will use for this class:
    ```conda install beautifulsoup4 bokeh hdf5 html5lib ipykernel jupyter ipython matplotlib matplotlib-base matplotlib-inline nltk notebook numpy openpyxl pandas pillow requests scikit-learn scrapy seaborn scipy statsmodels```
    and
    ```conda install -c plotly plotly=5.15.0```
    * Install some of the other packages that we'll be using:
    ```pip install streamlit```
---
### 3. VS Code
1. Download and install [VS Code](https://code.visualstudio.com/)
2. Install the following extensions.  To install an extension, click on the "Extensions" icon on the left most toolbar, search for the extension name in the search bar, and click the "Install" button.  
    * GitHub Pull Requests and Issues
    * Python (by Microsoft)
    * Jupyter (by Microsoft)
3. Sign into GitHub through VS Code by clicking on the "GitHub" icon on the left most toolbar and clicking "Sign in". (*Note: You will first need to sign up for a [GitHub](https://github.com) account if you don't have one already*.)

---
---
## Setup Github
1. Create a [Github](https://github.com/) account (if you haven't already done so)
2. Setup your Github profile:
    * Add a picture
    * Add your name
    * Add a brief bio
    * Create a [profile README](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/managing-your-profile-readme)
3. Grant Github access to your computer:
    In order for you to be able "push" changes from your computer to Github, your Github needs to recognize your computer as having permission to do so.  You will need to use ONE of the following methods:
    * OAuth token
    * [SSH keys]({{site.url}}/{{site.baseurl}}/resources/sshsetup)


    



