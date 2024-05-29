# blango

Blog Web Application, this is a practice project to work with Django-5.0.

## Installation

Create a virtual environment, using python3-venv:

```
$ mkdir blango
$ python3 -m venv env
```

Activate your virtual environment, you will see the environment in parenthesis in your command line:

```
$ source env/bin/activate
(env) $
```

Install the requirements:

```
(env) $ pip install requirements.txt
```

## Apps configuration and executing the DB migrations

Remember to include each app inside the INSTALLED_APPS list, in the blango/settings.py file.

```
INSTALLED_APPS = [
    ...,
    blog,
]
```

Then you need to build and run the migrations of the apps:

```
(env) $ python manage.py makemigrations
(env) $ python manage.py migrate
```

## Run the server

To run the project on the localhost server:

```
(env) $ python manage.py runserver 0.0.0.0:8000
```

Then in a browser you can access to your system putting in your search bar the url that connect with your server `localhost:8000`.

The available routes are:

/admin/