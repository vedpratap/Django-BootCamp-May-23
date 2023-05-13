# Django-BootCamp-May-23
Web Application Using Python Django.

## Day 01/03 (Topics Covered)
- Django Installation & Setting up a new project
- Run Django Development server
- Setting Up Views & URLs
- Templates, Static Assets, Template Inheritance
- GET vs POST
- Additional - Table for a number using jinja template

### Django Installation & Setting up a new project
- Go to the desired directory where you want to setup your project.
- Open `Command Prompt` there or any command line environment.
- First create Virtual Environment and activate it in the same directory.
  - `python -m venv .env` : It will create `.env` folder.
  - `.env\scripts\activate` : It will activate virtual environment.
  - `Note` : Python virtual environments give you the ability to isolate your Python development projects from your system installed Python and other Python environments. This gives you full control of your project and makes it easily reproducible.
- Install Django : `pip install django` - This will install Django framework.
- Run the command `django-admin` for checking proper installment of django. It will run smoothly in case of proper installation.
- Run the command `django-admin startproject projectname` : This will create projects (some directories) inside the folder as shown below. `projectname` can be anything. Example shown below using `myapp`
![Folder](images/folder_myapp.png)
- structure of folder
![Code](images/code_myapp.png)
- Explanations
  - `manage.py`
    - If you are not new to Django, you must have seen the word “command-line utility” many times. But what does this mean?
    - Well, by using the command-line utility, you can migrate i.e., either import or export metadata objects across different domains or setup. You can create one or more       objects within an object or its multiple objects. Now straight away coming to the topic. What is `manage.py`?
    - This file is used as a command-line utility for our projects. We will use this file for debugging, deploying, and running our web applications.
    - The file contains the code for running the server, makemigrations or migrations, and several other commands as well, which we perform in the code editor.
    - It performs the same things as django-admin but also provides some project-specific functionality. 
  - `__init.py_`
    - This is an empty file. The function of this file is to tell the Python interpreter that this directory is a package and involvement of this `__init.py_` file in it  makes it a python project.
  - `settings.py`
    - It contains the Django project configuration.
    - The setting.py is the most important file, and it is used for adding all the applications and middleware applications. This is the main setting file of the Django  project. 
    - This contains several variable names, and if you change the value, your application will work accordingly.
    - It contains sqlite3 as the default database. We can change this database to Mysql, PostgreSQL, or MongoDB according to the web application we create.
    - It contains some pre-installed apps and middleware that are there to provide basic functionality.
  - `urls.py`
    - URL is a universal resource locator, it contains all the endpoints that we should have for our website. It is used to provide you the address of the resources (images, webpages, websites, etc) that are present out there on the internet.
    - In simpler words, this file tells Django that if a user comes with this URL, direct them to that particular website or image whatsoever it is.
  - `wsgi.py`
    - When you will complete your journey from development to production, the next task is hosting your application. Here you will not be using the Django web server, but the WSGI server will take care of it.
    - WSGI stands for Web Server Gateway Interface, it describes the way how servers interact with the applications.
    - It is a very easy task, you just have to import middleware according to the server you want to use. For every server, there is Django middleware available that solves all the integration and connectivity issues. 
  - `asgi.py`
    - ASGI works similar to WSGI but comes with some additional functionality.  ASGI stands for Asynchronous Server Gateway Interface. It is now replacing its predecessor WSGI. 

### Run Django Development server
### Setting Up Views & URLs
### Templates, Static Assets, Template Inheritance
### GET vs POST
### Additional - Table for a number using jinja template
