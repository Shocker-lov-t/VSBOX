#Student Management System

This is a student management system built using * Django 4.0 * , * Amazon web services * and * Bootstarp5 *.

## Prerequisites(Install):

	1. Python 3.10.4
	2. Pycharm

## Setting Up AWS Server
From AWS Console go to Lightsail Service

	-> 	Launch a windows server
	->	setup inbound and outbound rules for https and tcp connections over 8000 port
	-> 	install python in the server
	-> 	migrate your code into the server

#setting up AWS Database (optional) 
From AWS Console go to RDS service

	-Launch an Postgresql Database instance and note down the username,master username and password of the instance ( it will be shown one time only so make sure to note them down very carefully)
    -Wait for the database instance to be in running state ( Takes approximately 10 min)
    -After Launched, click on the instance and it will show the details of your database
    -Open Django project's Settings.py file, there you will see a section "DATABASE" IN LINE 85 
          >>> Change name to the username to saved earlier
          >>> Change Username to master username
          >>> Change Password to new Password
          >>> Change Host to new host which is shown exactly on aws console database instance page
    -SAVE CHANGES

## Installation

From the **root** directory run:

	->	python -m venv venv
	->	venv\scripts\activate
	->	pip install -r requirements.txt
	->	python manage.py makemigrations
	->	python manage.py migrate
	->	python manage.py createsuperuser
		(When prompted, enter a username, email, and password.)

	->	python manage.py runserver 0.0.0.0 (for local host) or 0.0.0.0:8000 (for global host)


## View the application

Go to http://127.0.0.1:8000/ to view the application for local host <br>
OR<br>

Go to http://{Lightsail_IP}:8000/ to view the application for global host

Thank You.
