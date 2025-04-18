# Python Style Guide
A quick guide on few general and specific guidelines in Python   
Based on PEP 8 Style Guide : https://peps.python.org/pep-0008/ or https://pep8.org/

## General Guidelines

* Limit each line to 80 characters
* Indent using 4 Spaces
* Keep object and variable names as descriptive as possible   
  Prioritize well descriptive variable names over use of explanatory comments
* Follow appropriate naming cases [Reference](https://github.com/Santosh-GS/programming-notes/blob/main/python_naming_cases.md)
* Be consistent with single and double quotes for characters and strings
* Conventionally, use `self` for method, `cls` for classmethod, `*args` and `**kwargs`
* Seperate any top level classes and function with 2 blank lines and nested ones with 1 blank line
* Avoid deep nesting of conditionals or loops whenever possible
* Single Responsibility Principle:   
  Try to give single task for a function or object   
  Prefer multiple small tasked functions over a long multi tasking function
* Assign variables or a data structure to repeatedly used values to allow easier modifiications later   
  <br>
* Import everything at top and import one module per line (after module docstring)
* While importing from a single module, import multiple in the same line  
  `from os import path, stat`
* Avoid wilcard import (importing everything from a module)  
  `from os import *` **(Don't do this)**
* Import alphabetically, first std libraries and then the user defined ones  
  <br>
* Use triple double-quotes for docstring
* Module docstring goes before imports
* Start writing docstring content in the same line of triple quotes when only one-liner description is being given  
  `""" This is a single line docstring """`  
  `"""`  
  `Docstring in multiple lines`  
  `"""`  
  <br>
* Use 2 spaces before `#` for in-line comments and 1 space after `#`
* A white space goes after a comma except in case of a trailing comma or closing parantheses   
  `foo = (0,)`  
  `my_list = [1, 2, 3]`
* Preferably use one space around operators  
  Except while showing precedence of operators and for default values in function parameter declaration  
  `final_sum = a*b + c*d`  
  `def my_color_function(color="black", imag=0.0):`   
  <br>
* Use `is` instead of `==` while checking for `None`  
  `x = None`  
  `if x is None: do_this()`
* `if foo is not x:`  
  `if not foo is x:` (equivalent to `not (foo is x)` but not `(not foo) is x`)  
  both are equivalent but prefer the former one as `is not` kinda acts like a single operator  
  <br>
* Always catch specific exceptions in `try`-`except` statements rather than using `except Exception:`   
  <br>
* `if foo.startswith("bar"):`  (Preferred)  
  `if foo[:3] == "bar":`  
  prefer `.startswith` or `.endswith` instead of slice (allegedly for better accuracy and performance)  

### References:
[Write Python Code Properly!](https://www.youtube.com/watch?v=D4_s3q038I0)   
[My 5 "Clean" Code Principles](https://www.youtube.com/watch?v=kfyo-N-xAwE)   

### Full Guide:
A comprehensive style guide is available at https://gist.github.com/RichardBronosky/454964087739a449da04
