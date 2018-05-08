=======================
medialog.mobilethemeOne
=======================


Introduction
============

``medialog.mobilethemeOne`` is an installable Plone Mobile Theme developed by 
`Grieg Medialog AS`_ using the **theming** and **packaging** features available 
in `plone.app.theming`_ and `zettwerk.mobiletheming`_ packages.


Screenshots
===========

Layout of the site when viewed in a computer resolution:

.. figure:: image:: https://github.com/espenmn/medialog.mobilethemeOne/raw/master/medialog/mobilethemeOne/static/preview.png

  medialog.mobilethemeOne Mobile Theme


Features
========

- It's an Mobile Theme with responsive design support.
- It's an installable Plone Theme package.
- After installation from Add-ons controlpanel, this theme is enabled automatically.
- Also it's a simple Diazo package (Zip file).


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest version (https://plone.org/download)
- The ``plone.app.theming`` and ``zettwerk.mobiletheming`` packages (*will be installed as a dependencies of this package*)


Installation
============


Zip file
--------

If you are an end user, you might enjoy installation via zip file import.

1. Download a `zip file <https://github.com/espenmn/medialog.mobilethemeOne/raw/master/medialog.mobilethemeOne.zip>`_.
2. Import the theme from the Diazo theme control panel.

Enabling the theme
^^^^^^^^^^^^^^^^^^

Select and enable the theme from the Diazo control panel. That's it!


Buildout
--------

If you are a developer, you might enjoy installing it via buildout.

For install ``medialog.mobilethemeOne`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        medialog.mobilethemeOne


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'medialog.mobilethemeOne',
    ],


Usage
=====

A theme intended for use with mobile theming control panel (``zettwerk.mobiletheming``).

You probably want to use the theme like this:

- install ``zettwerk.mobiletheming`` package

- install ``medialog.mobilethemeOne`` package

- go to the mobile theming control panel and choose which url that should have the mobile theme.

- It is of course possible to enable the theme in diazo theme control panel and use it as a regular theme


When you want to edit the theme, you should do this on the file system.
If you duplicate it TTW, the overridden templates will not be used.


Contribute
==========

- Issue Tracker: https://github.com/espenmn/medialog.mobilethemeOne/issues
- Source Code: https://github.com/espenmn/medialog.mobilethemeOne


License
=======

The project is licensed under the GPLv2.

Credits
-------

Author
^^^^^^

- Espen Moe-Nilssen (espen at medialog dot no), Grieg Medialog AS.

.. _`Grieg Medialog AS`: http://www.medialog.no/
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
.. _`zettwerk.mobiletheming`: https://github.com/collective/zettwerk.mobiletheming
