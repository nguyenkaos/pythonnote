Code Style & Run
---------------------



Run Python
^^^^^^^^^^^^^^^^^^^^^^^^


**Text Editor**
I
Sublime text
vim
NotePad++
Pycharm

    
 To run a script in python, just type *python script.py* , then our program will compile and run at the same time 
 
.. Note:: In fact, python use a program, called the interpreter (`/usr/bin/python` in Linux or `python.exe` in Window) to compile our source code to the bytecode ``*.pyc``, then execute this bytecode.


Python option run
^^^^^^^^^^^^^^^^^^^^^^^^

We mostly use :class:`python -m mymodule` to run a python source code . But there are other common command-lines options :

.. code:: python

    python [-c command | -m module-name | script | - ] [args]



**-c**

The -c cmd option can be used to execute short programs in the form of a command-line option—for example:

.. code:: python 

    $ python -c "print('hello world')".
    hello world

**-m** 

Runs a library module as a script which executes inside the :class:`__main__` module prior to the execution of the main script.
For this command, example  :class:`python -m mymodule` : Python does 2 things : 

    - First, import the packages :class:`mymodule`. If the given module isn't located on the Python module path, an error is handled here and the program will be stop.

    - Second, run this module :class:`mymodule` like as a script.


Exemple : I have a script **foo.py**

.. code:: python 

    print 'hello'
    print __name__
    
then we run this script by 2 ways:

.. code:: python

    $ python foo.py
    hello
    __main__
    $ python -m foo
    hello
    __main__

We have the same result.
Attention with the path to our module, it raise an error if the module isn't in the PYTHON_PATH.We shall see it at `sys path <Operating_System_Modules.html#syspath>`_ 

*What's the use?* 



**-i** 

Python -i means to keep the terminal running after the script finishes. We might use this to examine global variables for debugging.


    
Write Python code correctly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^


Indentation
================



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






