Run Python Script
---------------------



Run Python
^^^^^^^^^^^^^^^^^^^^^^^^
    
 To run a script in python, just type *python script.py* , then our program will compile and run at the same time 
 
.. Note:: In fact, python use a program, called the interpreter (`/usr/bin/python` in Linux or `python.exe` in Window) to compile our source code to the bytecode ``*.pyc``, then execute this bytecode.


Python Interactive
^^^^^^^^^^^^^^^^^^^^^^^^

The Python interpreter is usually installed at the path of python installation. To open this, juste typing ``python`` to the shell, we have :

.. code:: python
    
    $ python
    Python 2.7.9 (default, Mar  1 2015, 12:57:24)
    [GCC 4.9.2] on linux2
    Type "help", "copyright", "credits" or "license" for more information.
    >>>
    
and from now, we can apply and test all python commands here !!

.. Tip::  For me, this tool is very important on my work. When I write a new function, always I test it directly on Interactive Console with maximum testcase possible. This way helps me avoid many stupid mistakes.

    
Python command options
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

We have the same result ! 
Attention with the path to our module, it raise an error if the module isn't in the PYTHON_PATH.We shall see it at `sys module <Operating_System_Modules.html#syspath>`_ 

