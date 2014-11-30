Django Markdown Utils
============

A reusable Django app with some useful markdown utilities

Installation
------------

To get the latest stable release from PyPi

.. code-block:: bash

    pip install django-markdown-utils

To get the latest commit from GitHub

.. code-block:: bash

    pip install -e git+git://github.com/bitmazk/django-markdown-utils.git#egg=markdown_utils

TODO: Describe further installation steps (edit / remove the examples below):

Add ``markdown_utils`` to your ``INSTALLED_APPS``

.. code-block:: python

    INSTALLED_APPS = (
        ...,
        'markdown_utils',
    )

Add the ``markdown_utils`` URLs to your ``urls.py``

.. code-block:: python

    urlpatterns = patterns('',
        ...
        url(r'^/', include('markdown_utils.urls')),
    )

Before your tags/filters are available in your templates, load them by using

.. code-block:: html

	{% load markdown_utils_tags %}


Don't forget to migrate your database

.. code-block:: bash

    ./manage.py migrate markdown_utils


Usage
-----

TODO: Describe usage or point to docs. Also describe available settings and
templatetags.


Contribute
----------

If you want to contribute to this project, please perform the following steps

.. code-block:: bash

    # Fork this repository
    # Clone your fork
    mkvirtualenv -p python2.7 django-markdown-utils
    make develop

    git co -b feature_branch master
    # Implement your feature and tests
    git add . && git commit
    git push -u origin feature_branch
    # Send us a pull request for your feature branch