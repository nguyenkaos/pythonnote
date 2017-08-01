Python Code Style
---------------------


**Text Editor**

I recommend these text editors for python development :

    - Sublime text : very beautiful interface, Python syntax highlighting, Python plugins.
    - vim : for all *linuxer* :p
    - NotePad++ : I always use this editor although my friends mocking me :(( Having a perfect NppFPT for virtual machine, and mostly it has an option to backup all my source code each time I do Ctrl+S.
    - Pycharm : Full-featured IDE for Python. I tried it once, a very nice interface and efficient but it's so slow.



Indentation
================

**Whitespace 1**

    - 4 spaces per indentation level.
    - Never mix tabs and spaces.
    - One blank line between functions.
    - Two blank lines between classes.

**Whitespace 2**

    - Add a space after "," in ``dict``, ``list``, ``tuple``, & *argument lists*, and after ":" in dicts, but not before.
    - Put spaces around assignments & comparisons (except in argument lists).
    - No spaces just inside *parentheses* or just before argument lists.

Exemple:

    def make_squares(key, value=0):
        """Return a dictionary and a list..."""
        d = {key: value}
        l = [key, value]
        return d, l

Convention in Python for variable and function names
======================================================= 

- Class: ClassName
- Method name : method_name
- Function : names should be lowercase, with words separated by underscores as necessary to improve readability , example ``function_name``.
- Variables : lowercase with words separated by underscores as necessary to improve readability.
- global_var_name
- instance_var_name
- local_var_name
- function_parameter_name
- Constant name : GLOBAL_CONSTANT_NAME
- ExceptionName : ExceptionName

Docstrings & Comments
==========================

- Docstrings = Explain **how** to use code, and are for the users of our code. this must always have 3 things :

    + Purpose of the function 
    + Description the parameters (name, type, note), the return values (name, type, note), and any exceptions raised.
    + Un example to run this function
    
- Comments = explain **why**, and are for the maintainers of our code.



if __name__ == "__main__"
==========================


Sometimes we see this notion in source code, that means if we run directly the script from terminal, these command-lines in ``if`` block will be executed .By example we have a script **a.py** : 

.. code:: python 

    if __name__ == "__main__":
        print 'hello'

Then run in cmd:

.. code:: python 

    >>> python a.py
    hello
 

But if we import **a** into another script python, all commands in if ``__name__ == "__main__"`` will be not execute, because in this case, ``__name__`` become 'a'. Exemple we have the script **a.py** like as above, then we import **a.py** into **b.py**:

.. code:: python 
    
    import a
    if __name__ == "__main__":
        print 'hello b'
        print a.__name__

we run :

.. code:: python 
    
    >>> python b.py
    hello b
    a

*What's the use ?*

This thing's used for testing when we write a new module or new sub-script in a grand project. For my above exemple, I can write some testsuite after *if __name__ == "__main__":*






