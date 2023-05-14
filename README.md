AirBnB_clone
Project Description
The AirBnB clone project is a team effort to develop an AirBnB clone console, which aims to emulate the object management of AirBnB. The console utilizes JSON serialization and deserialization for object storage. It includes a directory with static web pages designed for both desktop and mobile, with ARIA implementation.

Getting Started
This project serves as the first step towards building a full web application. It is crucial because the concepts and code developed here will be used in subsequent projects such as HTML/CSS templating, database storage, API, and front-end integration. The tasks involved in this project are as follows:

Implement a parent class called BaseModel for initialization, serialization, and deserialization of future instances.
Create a simple flow of serialization/deserialization: Instance <-> Dictionary <-> JSON string <-> file.
Develop the necessary classes for AirBnB, including User, State, City, Place, etc., which inherit from BaseModel.
Create the first abstracted storage engine for the project: File storage.
Write unittests to validate all classes and the storage engine.
Execution
The console can be operated in both interactive and non-interactive modes. In interactive mode, the shell operates as follows:

$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$
In non-interactive mode, similar to the Shell project in C, you can use input redirection to pass commands to the console:
  
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
Testing
All tests are located in the tests folder of the project.

To execute all the tests, use the following command:

Modules
  
python3 -c 'print(__import__("my_module").__doc__)'

 Functions (inside and outside the classes)
  
  python3 -c 'print(__import__("my_module").my_function.__doc__)'
python3 -c 'print(__import__("my_module").MyClass.my_function.__doc__)'

  Classes
  
  python3 -c 'print(__import__("my_module").MyClass.__doc__)'

 All tests should also pass when executed in non-interactive mode:
  
  echo "python3 -m unittest discover tests" | bash

  
  
 
## Authors
- Michael Anokwulu
- Lydiah Kiboi
