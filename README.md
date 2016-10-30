link project https://godjango.com/41-start-your-api-django-rest-framework-part-1/

install pip
-----------
    sudo apt-get istall python-pip

install djangorestframework
---------------------------
    pip install django
    pip install djangorestframework
    pip install markdown       # Markdown support for the browsable API.
    pip install django-filter
    pip install pygments 

install httpie
--------------
    pip install httpie

install cookiecutter
--------------
    pip install cookiecutter
Getting started
===============
    cd ~
    django-admin.py startproject rest_backend
    cd rest_backend
    cookiecutter gh:agconti/cookiecutter-django-rest
    pip install PyJWT
    
    cd ~
    django-admin.py startproject tutorial
    cd tutorial
    Once that's done we can create an app that we'll use to create a simple Web API.
    
    python manage.py startapp snippets
    We'll need to add our new snippets app and the rest_framework app to INSTALLED_APPS. Let's edit the tutorial/settings.py file:
    
    INSTALLED_APPS = (
        ...
        'rest_framework',
        'snippets.apps.SnippetsConfig',
    )
