+++
authors = ["Karlo Kegljevic"]
title = "Python 3.8 released!"
date = "2019-10-16"
tags = ["python", "news"]
+++

## Assignment Expressions: The Walrus Operator

The arrival of the assignment expression, affectionately known as the "walrus operator" (:=), marks a paradigm shift in how we approach coding constructs. This operator allows us to perform assignments within other expressions, a seemingly small addition that unleashes a world of possibilities. The walrus operator finds its prime utility in loops and comprehensions, allowing developers to assign and utilize values within a single line of code.

```python
# Without the walrus operator
n = 0
while n < 10:
    print(n)
    n += 1

# With the walrus operator
n = 0
while n < 10:
    print((n := n + 1))
```

## Positional-Only Parameters: A New Syntax

Python 3.8 introduces a clear and concise syntax for defining positional-only parameters in function signatures. By using the `/` symbol, developers can indicate that specific parameters must be supplied solely through positional arguments and are not accessible as keyword arguments. This feature enhances the clarity of function usage and promotes code readability.

```python
def f(a, b, /, c, d, *, e, f):
    print(a, b, c, d, e, f)

# The following is a valid call:

f(10, 20, 30, d=40, e=50, f=60)

# However, these are invalid calls:

f(10, b=20, c=30, d=40, e=50, f=60)   # b cannot be a keyword argument
f(10, 20, 30, 40, 50, f=60)           # e must be a keyword argument
```


## f-strings Enhancements: Debugging Made Easier

The Python community's love for f-strings has led to improvements that cater to a developer's debugging needs. Python 3.8 brings the `=` specifier to f-strings, allowing developers to display both the expression and its value. This small yet impactful addition proves invaluable when debugging code and tracking variable values throughout program execution.

```python
>>> user = 'eric_idle'
>>> member_since = date(1975, 7, 31)
>>> f'{user=} {member_since=}'
"user='eric_idle' member_since=datetime.date(1975, 7, 31)"
```


---

### Embracing Python 3.8's Advancements

Python 3.8 propels the language forward with features that encapsulate the essence of Pythonic elegance and efficiency. The assignment expression (`:=`) liberates coding constructs, while positional-only parameters enhance function definition clarity. Additionally, f-strings with the = specifier serve as indispensable tools in a developer's debugging arsenal.

As you embark on your coding journey, consider incorporating these Python 3.8 features into your toolkit. Embrace the walrus operator's concise power, leverage the positional-only parameters for function clarity, and utilize f-strings with the = specifier to make debugging a breeze. With Python 3.8, you're equipped to navigate coding challenges with greater finesse and precision, embracing a language that continues to adapt and evolve to meet your programming needs.

So, update your interpreter, explore the new features, and let the innovations of Python 3.8 empower you to write more efficient and elegant code than ever before.