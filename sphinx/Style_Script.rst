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






