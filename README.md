#Student Management System

This is a student management system built using * Django 4.0 * , * Amazon web services * and * Bootstarp5 *.

## Prerequisites(Install):

1. Python 3.10.4
2. Pycharm
3. AWS Cli


## Installation(Local Host)

From the **root** directory run:

->	python -m venv venv
->	venv\scripts\activate
->	pip install -r requirements.txt
->	python manage.py makemigrations
->	python manage.py migrate
->	python manage.py createsuperuser

(When prompted, enter a username, email, and password.)

->	python manage.py runserver


## View the application

Go to http://127.0.0.1:8000/ to view the application.



## Installation(Global Hosting Using AWS)

#>>	Launch an Windows AWS Lightsail Instance
#>>	Migrate code into instance
#>>	Create new inbound rules with port number *8000*
#>>	Go to \student-management-system-master\student-management-system-master\django_project 
	
		>>>	Open * Settings.py * file.
		>>>	in * Allowed_Host * add your Lightsail Instance IP.

#>>	From the **root** directory run:

	->	python -m venv venv
	->	venv\scripts\activate
	->	pip install -r requirements.txt	
	->	python manage.py makemigrations
	->	python manage.py migrate
	->	python manage.py createsuperuser

		(When prompted, enter a username, email, and password.)
	->	python manage.py runserver
	->	python manage.py runserver 0.0.0.0:8000


## View the application

Go to http://{Your_LightSail_IP}:8000/ to view the application on Any Device.

Thank You.
