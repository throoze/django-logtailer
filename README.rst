=================================
Django LogTailer
=================================

:Version: 0.3.1
:Source: http://github.com/fireantology/django-logtailer/
--


Allows the viewing of any log file entries in real time directly from the Django admin interface.
It allows you to filter on logs with regex and offer also a log clipboard for save desired log lines to the django db.
This is a first beta version, don't expect so much.

Demos
========
- Demo `Video`_

.. _`Video`: http://www.vimeo.com/28891014

Requirements
========

- Django 1.3
- Sessions enabled

Installation
========

- Copy the logtailer folder in you project and add it to the INSTALLED_APPS
- add to urls.py: url(r'^logs/', include('logtailer.urls')),
- Run manage.py syncdb for create the required tables
- Run manage.py collectstatic

SETTING OPTIONS AVAILABLE
========

 - LOGTAILER_HISTORY_LINES , Number of line to get back from the file on first read, default value is 0

CHANGELOG
========

- updated urls.py to work on django >=1.6. 'django.conf.urls.defaults' no longer used.  