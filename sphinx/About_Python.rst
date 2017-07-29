About Python
---------------------

 
**What's Python ?**

- Python is an interpreted language, it is not a compiled language. This means that it needs to be run by another program, called the interpreter (`/usr/bin/python` in Linux or `python.exe` in Window) to generate the bytecode ``*.pyc``, rather than the processor itself. Not like as C, which runs directly on the processor, after a compilation to bytecode. 

- Because of interpreted languages, Python is a high-level programming language. For exemple, an important feature of high-level programming language is *garbage collector*, which free automatiquement the variable on memory at the end of program or function, to avoid memory leak.

- In France, in 2017, python becomes the best programmation language (after this `french site <https://www.developpez.com/actu/150166/IEEE-Python-devient-le-meilleur-langage-en-2017-en-depassant-C-et-Java-decouvrez-le-classement-complet-selon-divers-criteres/>`__ )
  
 
**Compare Python and other language**

This discussion is very huge on the internet, and there's some notes :

+---------------------+--------------------------------------------+------------------------------------+
|    Feature          |            |  Python                       |              | C                   |
|                     |                                            |                                    |
+=====================+============================================+====================================+
| Pointer             | | In python we dont have the definition    |            | Yes                   |
|                     | | of pointer. All variables are names      |                                    |
|                     | | bound to objects ! We will speak it at   |                                    |
|                     | | topic  `pointer <Types.html#pointer>`_ . |                                    |
+---------------------+--------------------------------------------+------------------------------------+
| Type                | | Dynamic ! we can change object type      | | Static typing !                  |
|                     | | type of variables at run-time            |                                    |
+---------------------+--------------------------------------------+------------------------------------+
| Varaible location   | | All objects in python stock in **heap**  | | We can define where we           |
|                     | | (whatever ``int``, ``float``...). Only   | | want to                          |
|                     | | the name of variable sits in **stack**   | | stock via pointer                |
+---------------------+--------------------------------------------+------------------------------------+
| Memory              | | Very inefficient !                       | | Very efficient !                 |
| & Performance       | | Example, a list [1,2,3] take 200 bytes.  | | Ex, a list {1,2,3} take          |
|                     | |                                          | | only 16 bytes                    |
|                     | | Slowly !                                 | | Fast !                           |
+---------------------+--------------------------------------------+------------------------------------+

 


**Python 2.7**

- This version is the most stable release, and  the most frequently used. This is scheduled to be the last major version in the 2.x series before it moves into an extended maintenance period. For me, I always work with version 2.7, so all of my notes in this site go with this version.  

- We must know that in 2020, python 2.7 will be not supported anymore and all modules will be released only for python3 :( Sometimes I try it, but the syntax is very different from version 2 but we have no choice, so now this's time to move to python 3 ! I advise that if we start a project now, we should try & work with version 3 with their packages/modules, and our project will be safe in 2020 :) 

- To show the current python using, on linux, we do

.. code:: python

    $ ls -l /usr/bin/python
    /usr/bin/python -> python2.7


