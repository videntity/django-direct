==============================================================
django-direct - A RESTFul API for Direct Certificate Discovery
==============================================================

django-direct is a simple Django application that provides a RESTFul 
API to validate and fetch Direct x509 certificate via LDAP and DNS.

Detailed documentation for using the API is in the "docs" directory. 
Installation instructions are below.

Quick start
-----------

1. Pip install django-direct::

    pip install django-direct


2. Add "direct" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = (
        ...
        'direct',
    )

3. Include the direct URLconf in your project urls.py like this::

    url(r'^direct/', include('direct.urls')),


4. Add the static content to your app::

   python manage.py collectstatic

5. There are no models in this application so there is no migration step.

6. Use the APIs.  Visit http://127.0.0.1:8000/direct/ to verify the installation and for more information.  
See the docs folder for more information.


Production configuration is out of scope fo this document. See https://docs.djangoproject.com/en/1.9/howto/deployment/ for more info.

