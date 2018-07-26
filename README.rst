=======================
diazoframework.skeleton
=======================


Introduction
============

``diazoframework.skeleton`` package provides the diazo framework implementation of the 
`Skeleton CSS framework`_ using the **theming** and **packaging** features available in the 
`diazoframework.plone`_ core package for create `Diazo`_ theme using `plone.app.theming`_.

They are useful for creating themes based on `Skeleton CSS framework`_. For documentation 
on the framework itself, check the website.

A Diazo framework should provide the framework resources and diazo rules to reuse 
and add to in a Diazo theme.


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest version (https://plone.org/download)
- The ``plone.app.theming`` package (*You will need enable it via "Add-ons" control 
  panel to use this package*)
- The ``diazoframework.plone`` package (*You will need enable it via "buildout" 
  configuration to use this package*)


Features
========

- This support the *Skeleton CSS* v1.2 resources.
- Included Diazo rules for the ``head``, ``portlets`` and ``structures`` *Skeleton* CSS styles.


Installation
============

This add-on can be installed has any other add-ons. It's doesn't have any profile, so 
just add it to your Zope instance, for doing that please the follow steps: 


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

Resources
=========

The resources of this framework can be reached through 
``/++framework++skeleton`` and there are placed at 
``diazoframework.skeleton/diazoframework/skeleton/framework/`` 
directory with following resources files:

::

    _ images
      _ apple-touch-icon-114x114.png
      _ apple-touch-icon.png
      _ apple-touch-icon-72x72.png
      _ favicon.ico
    _ index.html
    _ preview.png
    _ stylesheets
      _ base.css
      _ layout.css
      _ skeleton.css
    _ rules
      _ head.xml
      _ portlets.xml
      _ structures.xml


Current themes
==============

The `diazoframework.skeleton`_ package have the following themes:

`diazotheme.skeleton`_
    which contains themes that can both be used as starters for your own *Skeleton* based theme.


For more frameworks see: the `diazoframework.plone`_ package.


Contribute
==========

- Issue Tracker: https://github.com/TH-code/diazoframework.skeleton/issues
- Source Code: https://github.com/TH-code/diazoframework.skeleton


License
=======

The project is licensed under the GPLv2.

The *Skeleton CSS framework* is licensed under the MIT license.


Credits
-------

- Thijs Jonkman (t.jonkman at gmail dot com).


Amazing contributions
---------------------

- Leonardo J. Caballero G. aka macagua (leonardocaballero at gmail dot com).

You can find an updated list of package contributors on https://github.com/TH-code/diazoframework.skeleton/contributors


.. _`Skeleton CSS framework`: http://www.skeleton.co.uk/
.. _`diazoframework.plone`: https://github.com/collective/diazoframework.plone#current-frameworks
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
.. _`diazoframework.skeleton`: https://github.com/TH-code/diazoframework.skeleton
.. _`diazotheme.skeleton`: https://github.com/TH-code/diazotheme.skeleton
