About Python
---------------------

**What's Python ?**

- Python is an interpreted language, it is not a compiled language. This means that it needs to be run by another program, called the interpreter (`/usr/bin/python` in Linux or `python.exe` in Window) to generate the bytecode ``*.pyc``, rather than the processor itself. Not like as C, which runs directly on the processor, after a compilation to bytecode. 

- Because of interpreted languages, Python is a high-level programming language. For exemple, an important feature of high-level programming language is *garbage collector*, which free automatiquement the variable on memory at the end of program or function, to avoid memory leak.

- In France, in 2017, python becomes the best programmation language (after this `french site <https://www.developpez.com/actu/150166/IEEE-Python-devient-le-meilleur-langage-en-2017-en-depassant-C-et-Java-decouvrez-le-classement-complet-selon-divers-criteres/>`__ )
  
 
**Compare Python and other language**

This discussion is very huge on the internet, and there's some notes :
  
- Very simple syntax. The easiest syntax, and readability are stated design goals of the language and it goes to great lengths to maintain that. For example, we have to write 

- Does Python have *pointer* like as C ? No, python don't have definition of pointer. **All variables are names bound to objects** ! We will speak at topic `pointer <Types.html#pointer>`_ .

- Performance : We all know that Python was written in C, which is very powerful language because it runs straigth off on the memory, that why we never speak at this topic. But I think it depends on the way to implement the algorithm of developer.
 


**Python 2.7**

- This version is the most stable release, and  the most frequently used. This is scheduled to be the last major version in the 2.x series before it moves into an extended maintenance period. For me, I always work with version 2.7, so all of my notes in this site go with this version.  

- We must know that in 2020, python 2.7 will be not supported anymore and all modules will be released only for python3 :( Sometimes I try it, but the syntax is very different from version 2 but we have no choice, so now this's time to move to python 3 ! I advise that if we start a project now, we should try & work with version 3 with their packages/modules, and our project will be safe in 2020 :) 



**Pointer** 


.. code:: python

    >>> i = 5
    >>> j = i
    >>> j = 3
    >>> print(i)
    5

We see that ``i`` refers to an integer on memory has value 5 at first line, then ``j`` refers to ``i``, means ``j`` also refers to 5. But when we change ``j`` =3, that means ``j`` points to another location on memory. Because ``i`` is an integer which is an immutable object, so there'is not any change on ``i``. And whats about mutable object *list* ? 

.. code:: python

    >>> a = [1]
    >>> b = a
    >>> a[0] = 2
    >>> b[0]
    2

If 2 *lists* ``a`` and  ``b`` refer at same object, when ``a`` changes, ``b`` changes also !    