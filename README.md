# Django_REST_framework

# Create the project directory

    mkdir tutorial
    cd tutorial

# Create a virtual environment to isolate our package dependencies locally

    python3 -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`

# Install Django and Django REST framework into the virtual environment

    pip install djangorestframework

# Set up a new project with a single application

    django-admin startproject tutorial .  # Note the trailing '.' character
    cd tutorial
    django-admin startapp quickstart
    cd ..

# for runnig

    python3 manage.py runserver

# for migrate

    python manage.py migrate

# We'll also create an initial user named admin with a password. We'll authenticate as that user later in our example.

    python manage.py createsuperuser --username admin --email admin@example.com