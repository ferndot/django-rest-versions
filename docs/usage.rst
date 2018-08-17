=====
Usage
=====

To use django-rest-versions in a project, add it to your `INSTALLED_APPS`:

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
