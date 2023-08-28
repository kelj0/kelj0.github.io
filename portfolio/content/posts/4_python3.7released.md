+++
authors = ["Karlo Kegljevic"]
title = "Python 3.7 Released!"
date = "2018-06-27"
tags = ["python", "news"]
+++

Python 3.7 has been released! This release includes a number of new features and improvements, including:

* A new f-string syntax for string formatting
* A new walrus operator (`:`) for tuple unpacking
* A number of performance improvements

For more information, see the [Python 3.7 release notes](https://docs.python.org/3/whatsnew/3.7.html).

## New f-string syntax

The f-string syntax is a new way to format strings in Python. It is similar to the old format() syntax, but it is more concise and easier to read.

For example, the following code:

```python
>>> print("The value is {}".format(10))
The value is 10
```

can be written as:

```python
>>> print(f"The value is {10}")
The value is 10
```

The f-string syntax is also more powerful than the old format() syntax. For example, it can be used to insert variables, expressions, and even other strings into a string.

The code in the blog post should be formatted as follows:

```python
>>> print(f"The value is {10}")
The value is 10
```


The f-string syntax is enclosed in curly braces (`{}`), and the variable or expression to be inserted is placed inside the braces. For example, the code `print(f"The value is {10}")` inserts the value 10 into the string "The value is ...".

The f-string syntax can also be used to insert other strings into a string. For example, the code `print(f"The value is {'10'}")` inserts the string "10" into the string "The value is ...".

I hope this is helpful!