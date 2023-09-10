# learn_django
This repo will provide an outline for a django project

## Django installation in ubuntu
```sudo apt install python3-django```

## Create a project
```django-admin startproject {project_name} {dir}```

Each project will have following files,

1. {project_name}/
This is the actual Django project package

2. manage.py:
Entrypoint of the project which is responsible for managing various aspects of the project

3. settings.py:
Contains project specific settings

4. urls.py:
Define the url patterns of the project

5. __init__.py
Empty script which indicates the directory as a package

6. wsgi.py
Entry point of WSGI(Web Server Gateway Interface) application which is used to deploy the Django proj on production web servers.

7. asgi.py
Entry point of ASGI(Asynchronous Server Gateway Interface) application which is used to run the project with asynchronous web servers.

We can create multiple projects using **django-admin** command. But each project will have the its own settings, database and other project specific configurations

## Create a virtual environment for python packages:

```
virtualenv {virtual_env_name} -p {python_interpreter}
```

## Run the server
```python manage.py runserver```

## Create an app to the existing project
```django-admin startapp {app_name}```

Then, we need to add app name inside settings.py file under the INSTALLED_APPS to indicate the app is part of the existing project