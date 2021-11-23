## Django quick start app

###  [Getting started with Django](https://www.djangoproject.com/start/) - Basic application

- Download and install [Python](https://www.python.org/downloads), if not installed.
- Install [django python package](https://pypi.org/project/Django)
> pip install Django
- Create application
> django-admin startproject mysite
- Migrate the pre-installed apps to use them with your project
> python manage.py migrate
- Create admin user
> python manage.py createsuperuser
- Run the application. If port is not specified, default is 8000
> python manage.py runserver 8080
- Access the admin application in browser http://127.0.0.1:8080/admin/
- Access the basic application in browser http://127.0.0.1:8080/polls/

### Some commands used during this app development
- Create new app polls inside base app
> python manage.py startapp polls
- Generate the model SQLs before migrate
> python manage.py sqlmigrate polls 0001
- Migrate the change to use
> python manage.py migrate
- After changing models(in models.py) migrate those changes
> python manage.py makemigrations 
- Apply model changes to the database
> python manage.py migrate
- Test the polls app
> python manage.py test polls
