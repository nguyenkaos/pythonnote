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

The most common command-line options : 

*-m* : runs a library module as a script which executes inside the __main__ module prior to the execution of the main script.
python -m mymodule : Python does 2 things : first, import the packages *mymodule*, then runs library module *mymodule* as a script.
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


*-i*

python -i : Enters interactive mode after program execution. This option starts an interactive session immediately after a program has finished execution and is useful for debugging.

*-c*

The -c cmd option can be used to execute short programs in the form of a command-line option—for example:

.. code:: python 

    python -c "print('hello world')".


*-3*


*-t*

-t Reports warnings about inconsistent tab usage.
    
    
    
    
    




    
Write Python code correctly
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

**if __name__ == "__main__"**
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

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






