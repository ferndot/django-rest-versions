=============================
django-rest-versions
=============================

.. image:: https://badge.fury.io/py/django-rest-versions.svg
    :target: https://badge.fury.io/py/django-rest-versions

.. image:: https://travis-ci.org/joshua-s/django-rest-versions.svg?branch=master
    :target: https://travis-ci.org/joshua-s/django-rest-versions

.. image:: https://codecov.io/gh/joshua-s/django-rest-versions/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/joshua-s/django-rest-versions

Easy API versioning for Django Rest Framework

Documentation
-------------

The full documentation is at https://django-rest-versions.readthedocs.io.

Quickstart
----------

Install django-rest-versions::

    pip install django-rest-versions

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'rest_versions.apps.RestVersionsConfig',
        ...
    )

Add django-rest-versions's URL patterns:

.. code-block:: python

    from rest_versions import urls as rest_versions_urls


    urlpatterns = [
        ...
        url(r'^', include(rest_versions_urls)),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox

Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
