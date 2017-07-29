Variable Types 
---------------------





Built-In Types : 12

Pointer
^^^^^^^^^^
.. _pointer:

.. code:: python

    >>> i = 5
    >>> j = i
    >>> j = 3
    >>> print(i)
    5

We see that ``i`` refers to an integer on memory has value 5 at first line, then ``j`` refers to ``i``, means ``j`` also refers to 5. But when we change ``j`` =3, that means ``j`` points to another location on memory. Because ``i`` is an integer which is an immutable object, so there'is not any change on ``i``. And whats about mutable object *list* ? 

.. code:: python

    >>> a = [0, 1, 2, 3, 4]
    >>> b = a
    >>> b[2] = 9999
    >>> a
    [0, 1, 9999, 3, 4]

If 2 *lists* ``a`` and  ``b`` refer at same object, when ``a`` changes, ``b`` changes also !

Basic
^^^^^^^^^^^^^^^

Tips 
^^^^^^^^^^^^^^^

