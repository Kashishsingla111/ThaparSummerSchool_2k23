Resources:- https://techvidvan.com/tutorials/django-project-structure-layout/

IMAGE PENDING


# Part 1-
In test_project  we have 2 folders namely test_app and test_project(main project folder)
  image

# Part 2-
## In the inner test_project folder:-
image
### 2.1. manage.py
This file is used as a command-line utility for our projects. We will use this file for debugging, deploying, and running our web applications.


### 2.2. setting.py
The setting.py is the most important file, and it is used for adding all the applications and middleware applications. This is the main setting file of the Django project.


### 2.3. urls.py
URL is a universal resource locator, it contains all the endpoints that we should have for our website. In simpler words, this file tells Django that if a user comes with this URL, direct them to that particular website or image whatsoever it is.


# Part 3-
## In the  test_app folder:-


### 3.1. models.py<br>
Models.py represents the models of web applications in the form of classes.
Models define the structure of the database. It tells about the actual design, relationships between the data sets, and their attribute constraints. 


### 3.2. admin.py<br>
Admin.py file is used for registering the Django models into the Django administration.


### 3.3. views.py<br>
Views provide an interface through which a user interacts with a Django web application.

