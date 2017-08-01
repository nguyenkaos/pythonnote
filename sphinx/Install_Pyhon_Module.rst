Install Python & Package
-------------------------------

Install Python 
^^^^^^^^^^^^^^^^^

*Linux*

Gererally, python is installed by default in Linux OS at the path */usr/bin/python*. To find this path, there are many ways, for me I like :

.. code:: python

    $ which python
    /usr/bin/python

*Window*

To isntall python, we do these steps:

 - Download python installation at this (`site <https://www.python.org/downloads/>`__). Select the version you need to.
 
 - Double click on the downloaded file, then click next next ... to install. You can choose the specific directory also. For me I put it as default directory *D:\Python27*
 
 - To use easily, we should create a python environment variable on window :
 
    + Open Control Panel, then System
    
    + Click 'Advanced system settings' on the left
    
    + Click the 'Environment Variables' button
    
    + Under 'System variables' click the variable called 'Path' then the 'Edit...' button. (This will set it for all users, you could instead choose to edit the User variables to just set python as a command prompt command for the current user)
    
    + Without deleting any other text, add D:\Python27; (include the semi-colon) to the beginning of the 'Variable value' and click OK.
    
    + Click OK on the 'Environment Variables' window.

    
Install Module Python
^^^^^^^^^^^^^^^^^^^^^^^^^

 - As a popular open source development project, Python has an **active** supporting community of contributors and users that also make their software available for other Python developers to use under open source license terms. 

 - *This allows Python users to share and collaborate effectively*, benefiting from the solutions others have already created to common (and sometimes even rare!) problems, as well as potentially contributing their own solutions to the common pool.

 - **pip** is the preferred installer program. Starting with Python 3.4, it is included by default with the Python binary installers.

**Pip Installation**
 
*Linux*

To install python 

.. code:: python

    $ sudo apt-get install python-pip python-dev build-essential 
    $ sudo pip install --upgrade pip 
    $ sudo pip install --upgrade virtualenv 


*Window*

With the current python vesion, *pip* is located at <path_to_python_dir>/Python27/Scripts/
We see pip.exe : that is pip application. So to use easily, we should create a environement variable. Unless, each time we want to install a package, navigating to pip directory, and typing the pip commands.



**Basic Usage**

To install the package, you can use the following command : 
    
- Search a package :
    
    $pip search package_name

- Install :

    $pip install package_name

- Uninstall : 

    $pip uninstall package_name




