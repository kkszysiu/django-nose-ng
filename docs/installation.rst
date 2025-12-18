Installation
------------

You can get django-nose-ng from PyPI with... :

.. code-block:: shell

    $ pip install django-nose-ng

Or using uv:

.. code-block:: shell

    $ uv add django-nose-ng

The development version can be installed with... :

.. code-block:: shell

    $ pip install -e git+https://github.com/kkszysiu/django-nose-ng.git#egg=django-nose-ng

Since django-nose-ng extends Django's built-in test command, you should add it to
your ``INSTALLED_APPS`` in ``settings.py``:

.. code-block:: python

    INSTALLED_APPS = [
        ...
        'django_nose',
        ...
    ]

Then set ``TEST_RUNNER`` in ``settings.py``:

.. code-block:: python

    TEST_RUNNER = 'django_nose.NoseTestSuiteRunner'
