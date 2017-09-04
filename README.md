# Blogger

A simple blogging engine built with Django.

## First Time Setup

Install [Python](https://www.python.org/). Then install the python packages to
setup a Python virtual environment.

    > pip install virtualenv virtualenvwrapper

Setup a new virtualenv

    > mkvirtualenv blogger
    (blogger) >

The prefix (blogger) indicates that you're in a python virtual environment
named "blogger". If the terminal is closed, the virtualenv will need to be
activated again.

    > workon blogger

While in the virtual environment, install the python packages required to
run blogger.

    (blogger) > pip install --upgrade -r requirements.txt

## Running Blogger

Before running blogger locally, the database may need to be created/migrated.

    (blogger) python manage.py migrate

Once the database is setup, run the server.

    (blogger) > python manage.py runserver

This will start a Python server running the project. Visit http://localhost:8000
to see blogger.

# Running Tests

Use the following command to run unit tests:

    (blogger) > python manage.py test
