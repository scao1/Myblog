---
layout:  post
title: Docstrings
---

When you buy new home appliances, they usually come with user manuals. You can learn the function of the machine and how to use these function from the manuals. In computer science, docstrings perform the similar roles as user manuals to explain what programs do and how to use them. They are string literal like a comment in the code and can easily be spotted by the triple quotes. We use doctrings in python functions as examples.


### Docstring structures
Here is one example in python. The part """ Add a and b together, return the value""" is a doctring. It explains the function my_fun is used to add a and b together. 

```python
def my_fun(a,b):
""" Add a and b together, return the value"""
return a + b
```

There are more detailed docstrings. The example below is a muti-line docstring used a format called PEP-8 style. It not only illustrate the main function, but also explain the arguments(input). It is generally used for more complicated functions.


```python
def my_fun(a,b):
""" 
Add a and b together, return the value
Argument: 
a - an int or float
b - an int or float 
"""
return a + b
```

Another common kind of muti-line docstrings is called scipy-style docstrings. Take a look at the example below. The scipy style contains more information like the types of input and output.

```python
def my_fun(a,b):
""" 
Add a and b together, return the value

Parameter
----------------
Parameter 1: int or float
take in a number

Parameter 2: int or float
take in a number

Returns
-------
int or float
sum of a and b

Examples
--------
>>> function_name(1,2)
3
"""
return a + b
```

The above three kinds of docstrings are the most common docstring structures. How can we bring out those docstrings when we want to use the function. You can use help(my_fun) to let them show up. See the example below.  

```python
>>>help(my_fun)

Help on function my_fun in module __main__:
my_fun(a, b)
Add a and b together, return the value
```


### Tools for automatic docstring generation
Writing docstring for a complex program is tedious work. Luckily, there are some available tools to automatically generate docstrings. Below is a list common ones.
* Sphinx <http://www.sphinx-doc.org/en/master/>
* pydoc <https://docs.python.org/3.7/library/pydoc.html>
* Doxygen <http://www.doxygen.nl>

*credit: <https://github.ubc.ca/MDS-2019-20/DSCI_511_prog-dsci_students/blob/master/lectures/lecture2.ipynb>*


### Writing docstrings is a good habit
Writing proper docstrings is really a good habit for the programmers. Explicit docstrings get you easily hands on the program and save your much time. It is also great help to other people using it.


