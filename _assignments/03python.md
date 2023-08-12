---
title: "Week 3: Python Basics Practice"
layout: single
author_profile: false
classes: wide
excerpt: Basic python practice
---

## Setup your blog in GitHub pages & practice 
1.  In a sensible place on your computer, create a directory where you will store all the files for your class blog.  You can call the directory whatever you want, but something like "Blog" or "386Blog" would be appropriate. 
2.  Open the folder you just created in VSCode. 
3.  Create a new file called `index.md`. 


[LinkedIn Learning class)[https://github.com/LinkedInLearning/python-essential-training-4314028]

## Python review questions.

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
**5. Write a Python function that accepts a string and calculates the number of upper case letters, the number of lower case letters, and the number of spaces.  The function should return a dictionary where the keys are "upper", "lower", and "space" and the value is the number of occurences.  See the example output below.**    
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

In [2]: word_lengths(s)

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
**7.  Write a python function that accepts an integer `n` (where 2 $\le$ `n` $\le$ 9) and returns a list of all the numbers between 0 and `n`00 that have an `n` in them AND are divisible by `n`.**  

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



----
**9.  Use a dictionary comprehension to create a dictionary where the keys are the numbers between 100 and 200 (inclusive) that are divisble by 10 and the value associated with each key is the key divided by 100.**

*Desired result*
```
Out[1]: {100: 1.0,
         110: 1.1,
         120: 1.2,
         130: 1.3,
         140: 1.4,
         150: 1.5,
         160: 1.6,
         170: 1.7,
         180: 1.8,
         190: 1.9,
         200: 2.0}
 ```



