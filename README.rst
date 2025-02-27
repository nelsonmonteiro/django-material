===============
Django Material
===============

Material design for Django.


IN ORDER TO REDUCE MAINTENANCE COST, THE PACKAGE FUNCTIONALITY HAS BEEN MOVED INTO THE django-viewflow

PLEASE, CONSIDE TO UPGRADE

$ pip install django-viewflow>=2.0.0b1


.. image:: https://img.shields.io/pypi/v/django-material.svg
    :target: https://pypi.python.org/pypi/django-material
.. image:: https://img.shields.io/pypi/wheel/django-material.svg
    :target: https://pypi.python.org/pypi/django-material
.. image:: https://img.shields.io/pypi/status/django-material.svg
    :target: https://pypi.python.org/pypi/django-material
.. image:: https://travis-ci.org/viewflow/django-material.svg
    :target: https://travis-ci.org/viewflow/django-material
.. image:: https://img.shields.io/pypi/pyversions/django-material.svg
    :target: https://pypi.python.org/pypi/django-material
.. image:: https://img.shields.io/pypi/l/Django.svg
    :target: https://raw.githubusercontent.com/viewflow/django-material/master/LICENSE.txt
.. image:: https://badges.gitter.im/Join%20Chat.svg
   :alt: Join the chat at https://gitter.im/viewflow/django-material
   :target: https://gitter.im/viewflow/django-material?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge


- Django-Material 1.10.x compatible with Django 2.2/3.0/3.1/3.2/4.0
- Django-Material 1.[8,9].x compatible with Django 1.11/2.0/2.1/2.2/3.0/3.1/3.2
- Django-Material 1.7.x compatible with Django 1.11/2.0/2.1/2.2/3.0/3.1
- Django-Material 1.6.x compatible with Django 1.11/2.0/2.1/2.2/3.0
- Django-Material 1.[3,4,5].x compatible with Django 1.11/2.0/2.1/2.2
- Django-Material 1.2.x compatible with Django 1.11/2.0
- Django-Material 1.1.x compatible with Django 1.8/1.9/1.10/1.11

Tested with:

.. image:: demo/static/img/browserstack_small.png
  :target:  http://browserstack.com/

Overview
========

- Forms - New way to render django forms

  * Strong python/html code separation
  * Easy redefinition of particular fields rendering
  * Complex form layout support

- Frontend - Quick starter template for modular admin-line applications development

.. image:: .screen.png
   :width: 400px


Demo
====

http://forms.viewflow.io/

To checkout and run open source demo version locally, you need to have
`git <https://git-scm.com/>`_ and `tox
<https://tox.readthedocs.io/en/latest/>`_ tools installed.

.. code:: bash

    git clone https://github.com/viewflow/django-material.git
    cd django-material

    TOXENV=py36-dj111 tox -- python manage.py migrate --settings=demo.settings
    TOXENV=py36-dj111 tox -- python manage.py loaddata demo/fixtures/* --settings=demo.settings
    TOXENV=py36-dj111 tox -- python manage.py runserver --settings=demo.settings

Then you can go to http://127.0.0.1:8000/integration/ and login with
`admin:admin` username and password to the demo site.


Documentation
=============

http://docs.viewflow.io/material_forms.html

License
=======

Django Material is an Open Source project licensed under the terms of the `BSD3 license <https://github.com/viewflow/django-material/blob/master/LICENSE.txt>`_

Django Material Pro with additional features has a commercial-friendly license. Check http:viewflow.io/pro/ for details.


Changelog
=========


1.10.0 2021-11-12
------------------

- Drop support for python 2.7
- Drop support for Django 1.11, Django 2.0, Django 2.1
- Add support for Django 4.0
- Keep viewset.queryset for detai and delete views
- Improve multiple ajax select
- Speed up model List View
