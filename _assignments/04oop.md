---
title: "NOT FINISHED - Week 4: Object-Oriented Concepts"
layout: single
author_profile: false
classes: wide
excerpt: Practice writing python classes and integrate OOP concepts with the functionality of the pandas library.
---


**Objective:**  
The goal of this assignment is to merge foundational concepts from object-oriented programming with the utility of the Pandas library. By the end, you should be able to create classes that can effectively interact with and manipulate Pandas data structures.

**Problem Statement:**  
You are a data analyst at a digital library. Your task is to design a system that can process, manipulate, and analyze data regarding different books available in the library.

**Data:**  
You're given a CSV file named `library_books.csv` with the following columns:
1. `ISBN`: Unique identifier for each book.
2. `Title`: Title of the book.
3. `Author`: Author of the book.
4. `Genre`: Genre the book belongs to (e.g., Fiction, Non-Fiction, Mystery, Sci-Fi).
5. `Pages`: Number of pages in the book.
6. `PublishedYear`: The year the book was published.

**Task 1:** Create a `Book` class

1. Attributes:
   - `ISBN`
   - `Title`
   - `Author`
   - `Genre`
   - `Pages`
   - `PublishedYear`

2. Methods:
   - `get_age()`: Returns the age of the book based on the current year.
   - `is_long()`: Returns `True` if the book has more than 300 pages, otherwise `False`.

**Task 2:** Create a `Library` class

1. Attributes:
   - `data`: A pandas DataFrame loaded from a provided CSV.

2. Methods:
   - `add_book()`: Takes an instance of `Book` and adds it to the dataframe.
   - `remove_book()`: Takes an ISBN and removes the corresponding book from the dataframe.
   - `get_books_by_author()`: Takes an author's name and returns a dataframe containing all books by that author.
   - `get_genre_count()`: Returns a series with the count of books in each genre.

**Requirements:**

1. Ensure you use appropriate encapsulation principles. Not all attributes should be directly accessible or mutable.
2. Your `Library` class should handle potential errors gracefully. For instance, attempting to remove a book that doesn't exist.

---

**Deliverables:**  

1. Write the Python code for the `Book` and `Library` classes in a file named `digital_library.py`.
2. Provide a separate Python script, `test_library.py`, that:
   - Creates instances of the `Book` class.
   - Initializes a `Library` using the CSV data.
   - Tests all methods of both classes to ensure they work as expected.

**Submission Instructions:**  

1. Ensure your code is well-commented.
2. Submit both the `digital_library.py` and `test_library.py` files.
3. Ensure your code is free of syntax errors and runs without issues.

---

**Rubric:**  

1. Correct implementation and functionality of the `Book` class: 25 points.
2. Correct implementation and functionality of the `Library` class: 50 points.
3. Appropriate use of Pandas functions and methods: 15 points.
4. Clarity, structure, and comments in the code: 10 points.

**Bonus:**  
For an extra 10 points, enhance the `Library` class with a method `get_books_summary()` that returns a dataframe with the following columns: `Title`, `Author`, `Pages`, and a new column `Description` which combines all previous columns in the format: "`Title` by `Author` is a `Pages` pages long book."

---
