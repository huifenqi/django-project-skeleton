{% comment "This comment section will be deleted in the generated project" %}

# django-project-skeleton

**django-project-skeleton** is a skeleton for Django projects. It provides a directory structure for Django projects during different environments.

## Structure

* apps - contains subfolders with specific functionality;
* configs - stores all configuration related scripts (newrelic, gunicorn, nginx, celery, mongdb, redis, etc);
* static - contains js, css, images, types/fonts
* templates - all your html files
* media - contains all upload files
* scripts - contains all scripts which used by support by `runscript` of django-extensions

## Usage

To use this repository just use the `template` option of [django-admin][1].

	$ django-admin startproject --template=https://github.com/huifenqi/django-project-skeleton/archive/master.zip --extension=md,ini [project_name]

To create new app: `python manage.py startapp [app_name]`

For different environments: `export DJANGO_SETTINGS_MODULE="[project_name].settings.production"`

## Django materials need to read

1. [https://github.com/rosarior/awesome-django][2]
2. [https://www.fullstackpython.com/django.html][3]
3. [https://www.quora.com/What-are-some-best-practices-for-Django-development][4]

{% endcomment %}

# {{ project_name }}

This project has the following basic apps:

* App1 (short desc)
* App2 (short desc)
* App3 (short desc)

## Installation

To set up a development environment quickly, first install Python 2. It
comes with virtualenv built-in. So create a virtual env by:

`mkvirtualenv {{ project_name }}`

Install all dependencies:

`pip install -r requirements.txt`

[1]:	https://docs.djangoproject.com/en/1.8/ref/django-admin/#startproject-projectname-destination
[2]:	https://github.com/rosarior/awesome-django
[3]:	https://www.fullstackpython.com/django.html
[4]:	https://www.quora.com/What-are-some-best-practices-for-Django-development