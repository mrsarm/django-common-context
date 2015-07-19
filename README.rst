Django Common Context Processors
================================

Django Common Context Processors provides useful shortcuts
for developing Django projects.

To use it, put in ``TEMPLATE_CONTEXT_PROCESSORS``:

.. code:: python

    TEMPLATE_CONTEXT_PROCESSORS = (
        #...
        'common_context.context_processors.site',
        'common_context.context_processors.settings',
        #...

If you use Django 1.8+, set the ``context_processors`` option in
the ``OPTIONS`` of a ``DjangoTemplates`` backend instead (see
`here <https://docs.djangoproject.com/en/1.8/ref/settings/#template-context-processors/>`_).

Then in any page if you need to print the *Site Name* use::

    {{ site.name }}

Or if you need to get the value of a Django Settings parameter::

    {{ settings.ANY_SETTINGS_VALUE }}


About
-----

This sources are available in
https://github.com/mrsarm/django-common-context

Author: Mariano Ruiz <mrsarm@gmail.com>

License: LGPL-3 (C) 2014-2015
