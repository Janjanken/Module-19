ITE 306 Module 19 Alcantara
===========================

Web Framework using Python Flask

We wil require two package to setup your environment. 

To Install `Flask`_  &  `virtualenv`_ open CMD and type the following commands: 

1. `virtualenv`_

.. code-block:: text

    pip install virtualenv
    
Once installed, new virtual environment is created in a folder.

.. code-block:: text

   mkdir newproj
   cd newproj
   virtualenv venv
    
.. _virtualenv: https://www.tutorialspoint.com/flask/flask_environment.htm

To activate corresponding environment, on Windows, use the following

.. code-block:: text

   venv\scripts\activate

2. `Flask`_  

We are now ready to install Flask in this environment.

.. code-block:: text

    pip install Flask

.. _Flask: https://www.tutorialspoint.com/flask/flask_environment.htm

myflask1.py
===========

Step 1: Test & Run
--------------------
To start, open `myflask1.py`_ and do the following:

.. code-block:: python

  from flask import Flask
  app = Flask(__name__)

  @app.route('/hello/<name>')
  def hello_name(name):
	return 'Hello %s!' % name

  if __name__ == '__main__':
	    app.run()


* copy/download `myflask1.py`_ 
* open CMD and type the `myflask1.py`_ file directory

It should be like the following:

.. code-block:: text

    C:\Users\Desktop>python C:\Users\Desktop\myflask1.py
    
The Output would be: 

.. code-block:: text
 
    * Serving Flask app 'myflask1'
    * Debug mode: off
    WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
    * Running on http://127.0.0.1:5000
    Press CTRL+C to quit

* copy the URL http://127.0.0.1:5000/ and paste it in your preferred browser tab
.. _myflask.py: https://github.com/JkAlcntr/ITE-MODULE-19-ALCANTARA/blob/main/myflask1.py
Step 2. TRY 
-----------
Now try this

Enter this URL http://127.0.0.1:5000/hello/<name>

replace <name> with your name.

Example: 

.. code-block:: text

   http://127.0.0.1:5000/hello/John

Output would display like this:

.. code-block:: text

    Hello John!

Good job!👍

myflash2.py
===========

Step 1. Download the pythontest folder or copy files located inside it.

Step 2. Repeat the procedure same as the above run the myflask2.py on cmd after that;

Step 3. Open login.html file in your selected browser

Step 4. Enter name 

.. image:: https://github.com/JkAlcntr/ITE-MODULE-19-ALCANTARA/blob/main/Capture.PNG

Step 5. Click Submit

Output will show:

.. code-block:: text

   Welcome John







