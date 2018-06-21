=======================
diazoframework.skeleton
=======================

This package provides the diazo framework implementation of the 
`Skeleton CSS framework`_. For documentation on the 
framework itself, check the website.


Introduction
============

``diazoframework.skeleton`` package using the **theming** and 
**packaging** features available in the `diazoframework.plone`_ core 
package for create Diazo_ theme using `plone.app.theming`_.


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest version (https://plone.org/download)
- The ``plone.app.theming`` package (*will be installed as a dependency of this package*)


Features
========

- This support the *Skeleton CSS* resources for version 1.2.
- Included Diazo rules for the ``head``, ``portlets`` and ``structures`` *Skeleton* CSS styles.


Installation
============


Buildout
--------

If you are a developer, you might enjoy installing it via buildout.

For install ``diazoframework.skeleton`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        diazoframework.skeleton


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'diazoframework.skeleton',
    ],


..
    Enabling the theme
    ^^^^^^^^^^^^^^^^^^

    Select and enable the theme from the Diazo control panel. That's it!


Themes that use it
==================

This framework is used by:

`diazotheme.skeleton`_
    which contains themes that can both be used as starters for your own *Skeleton* based theme.

For more frameworks see: the `diazoframework.plone`_ package.


Skeleton Resources
==================

The resources of this framework can be reached through 
``/++framework++skeleton`` and there are placed at 
``diazoframework.skeleton/diazoframework/skeleton/framework/`` 
directory with following resources files:

::

    framework/
    ├── images
    ├── index.html
    ├── preview.png
    ├── stylesheets
    └── rules
        ├── head.xml
        ├── portlets.xml
        └── structures.xml



Contribute
==========

- Issue Tracker: https://github.com/TH-code/diazoframework.skeleton/issues
- Source Code: https://github.com/TH-code/diazoframework.skeleton


License
=======

The project is licensed under the GPLv2.


Credits
-------

- Thijs Jonkman (t.jonkman at gmail dot com).
- Leonardo Caballero (leonardocaballero at gmail dot com).

.. _`Skeleton CSS framework`: http://www.skeleton.co.uk/
.. _`diazotheme.skeleton`: https://github.com/TH-code/diazotheme.skeleton
.. _`diazoframework.plone`: https://github.com/TH-code/diazoframework.plone#current-frameworks
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
