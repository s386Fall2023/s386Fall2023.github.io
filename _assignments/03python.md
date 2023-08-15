---
title: "Week 3: Python Basics Practice"
layout: single
author_profile: false
classes: wide
excerpt: Basic python practice
---

## Anaconda
In order to ensure that we are all running the same version of python and of the packages we'll be using, create a (conda) virtual environment for our class:
* In the terminal (Mac) or Anaconda prompt (Windows) type
    ```conda create --name stat386 python==3.10.12```
* Activate the environment you just created:
    ```conda activate stat386```
* Conda install the packages we will use for this class:
    ```conda install beautifulsoup4=4.12.2 bokeh=3.2.1 hdf5=1.12.1 html5lib=1.1 ipykernel=6.25.0 jupyter=1.0.0 ipython=8.12.2 matplotlib=3.7.1 matplotlib-inline=0.1.6 nltk=3.8.1 notebook=6.5.4 numpy=1.25.2 openpyxl=3.0.10 pandas=1.5.3 pillow=9.4.0 requests=2.31.0 scikit-learn=1.3.0 scrapy=2.8.0 seaborn=0.12.2 scipy=1.11.1 statsmodels=0.14.0```
    and
    ```conda install -c plotly plotly=5.16.0```
* Install some of the other packages that we'll be using:
    ```pip install streamlit```

## VS Code
1. Install the following extensions.  To install an extension, click on the "Extensions" icon on the left most toolbar, search for the extension name in the search bar, and click the "Install" button.  
    * GitHub Pull Requests and Issues
    * Python (by Microsoft)
    * Jupyter (by Microsoft)
2. Sign into GitHub through VS Code by clicking on the "GitHub" icon on the left most toolbar and clicking "Sign in". 

## Finish Blog Setup

1. If you haven't already, finish setting up your blog following [these instructions]({{site.url}}/{{site.baseurl}}/resources/blogsetup).
2. Once you have finished, add you


## Python review questions.
* Create a folder for this homework assignment in a sensible location on your computer
* Initialize the folder as a git repository either in the command line or with VSCode.
* Open the folder in VSCode (if you haven't already)
* Practice using VSCode with git while you complete the rest of the assignment.
* Make sure that you are using the class virtual environment 

**1.  Write a Python function that will compute the Euclidean distance between any two points.  The function should accept as input two tuples in the form of ((x<sub>1</sub>, y<sub>1</sub>),(x<sub>2</sub>, y<sub>2</sub>)) and return the Euclidean distance.**

*Example output:*

```
In [1]: euclid_dist((1,3),(7,11))
out[1]: 10
```

-----
**2. Write a Python function that computes the value of ``n + nn + nnn`` where ``n`` is an integer.  For example if,  ``n=2``, the function should return ``246`` (which is the sum of 2+22+222).**  

*Example output:*

```
In [1]: sum_ns(2)
Out[1]: 246
```

-----
**3. Write a Python function that determines if ``n`` is a perfect square, where ``n`` is an integer.  The function return either "False" or "n is a perfect square of x"  (where ``n`` and ``x`` are appropriate for the input).**

*Example output:*

```
In [1]: perfect_square(24)
Out[1]: False

In [2]: perfect_square(25)
Out[2]: 25 is a perfect square of 5
```

----
**4. Write a Python function that checks whether a string is a palindrome or not.  A palindrome is a word or phrase that reads the same forwards and backwards (ignoring spaces), such as "madam" or "nurses run".**

*Example output:*

```
In [1]: is_palindrome('madam')
Out[1]: True

In [2]: is_palindrome('nurses run')
Out[2]: True

In [3]: is_palindrome('starlight')
Out[3]: False
```

----
**5. Write a Python function that accepts a string and calculates the number of upper case letters, the number of lower case letters, and the number of spaces.  The function should return a dictionary where the keys are "upper", "lower", and "space" and the value is the number of occurrences.  See the example output below.**    
(Hint:  check out what methods are available for strings.)  

 *Example output:*

```
In [1]: count_letter_types("HELLO!! How are you today?")
Out[1]: {'upper': 6, 'lower': 13, 'space': 4}

```


----
**6. Write a Python function that accepts a string a returns a dictionary where the key word is a word length and the value is a list of all the words that are that word length.  See the example output below.**  

*Example output: (note, it's okay if the keys of your dictionary are in a different order)*

```
In [1]: s = "It is a truth universally acknowledged that a single man in possession of a good fortune must be in want of a wife"

In [2]: count_word_lengths(s)

Out[2]: {1: ['a', 'a', 'a', 'a'],
         2: ['It', 'is', 'in', 'of', 'be', 'in', 'of'],
         3: ['man'],
         4: ['that', 'good', 'must', 'want', 'wife'],
         5: ['truth'],
         6: ['single'],
         7: ['fortune'],
         10: ['possession'],
         11: ['universally'],
         12: ['acknowledged']}
```


----
**7.  Write a python function that accepts an integer `n` (where 2 $\le$ `n` $\le$ 9) and returns a list of all the numbers between 0 and `n`00 that have an `n` in them AND are divisible by `n`. See the example output below.**  

```
In [1]: n_list(3)
Out[1]: [3,
         30,
         33,
         36,
         39,
         63,
         ...
         300]

In [2]: n_list(10)
Out[2]: "Invalid input: enter a number between 2 and 9"
```


---
**8. Write a Python function that takes a list of numbers as input and calculates the sum of all even numbers in the list. Additionally, find the maximum value among these even numbers and determine how many times it appears in the list. Finally, print both the sum and the maximum value along with its frequency. See the example output below.**


```
In [1]: evens_mean_max([1,2,3,4,5,6])
Out[1]: The sum of the even numbers is 12.
        The maximum of the even numbers is 6 and it appears 1 time(s) in the list.

In [2]: evens_mean_max([1,7,2,3,7,4,5,6,7,6])
Out[1]: The sum of the even numbers is 18.
        The maximum of the even numbers is 6 and it appears 2 time(s) in the list.
```




