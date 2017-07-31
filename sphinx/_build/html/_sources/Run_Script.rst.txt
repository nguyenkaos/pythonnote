Run Python Script
---------------------



Run Python
^^^^^^^^^^^^^^^^^^^^^^^^
    
 To run a script in python, just type *python script.py* , then our program will compile and run at the same time 
 
.. Note:: In fact, python use a program, called the interpreter (`/usr/bin/python` in Linux or `python.exe` in Window) to compile our source code to the bytecode ``*.pyc``, then execute this bytecode.


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

Runs a library module as a script which executes inside the __main__ module prior to the execution of the main script.
For this command, example  :class:`python -m mymodule` : Python does 2 things : 

    - First, import the packages :class:`mymodule` if , then runs library module *mymodule* as a script. If the given module isn't located on the Python module path, an error is handled here and the program will be stop.
    
    - Second, run this module :class:`mymodule` like as a script.
    
    
Exemple : I have a script **foo.py**

.. code:: python 

    print 'hello'
    
then we run this script by 2 ways:

.. code:: python 

    $ python foo.py
    hello
    $ python -m foo
    hello
    
We have the same result ! 
Attention with the path to our module, it raise an error if the module isn't in the PYTHON_PATH.We shall see it at `sys module <Operating_System_Modules.html#syspath>`_ 
