Introduction
============

plone.app.discussion aims to be the new commenting system for Plone.
It was initially developed as part of the Google Summer of Code 2009
by Timo Stollenwerk (student) and Martin Aspeli (mentor).

For details on the progress of this project, visit our `Pivotal Tracker`_.

.. _`Pivotal Tracker`: http://www.pivotaltracker.com/projects/15135

Feel free to send bug reports and feature requests to timo@zmag.de.

Disclaimer
==========

This is an alpha release! Alpha releases should only be used for testing and development.

Requirements
============

Plone 3.3 or later.

Buildout Installation
=====================

To install plone.app.discussion, add the following code to your buildout.cfg::

    [buildout]
    ...
    extends =
        ...
        http://good-py.appspot.com/release/plone.app.discussion/1.0a1

    ...

    [instance]
    ...
    eggs =
        ...
        plone.app.discussion

    ...


Add-on Products
===============

- `collective.autoresizetextarea`_ (for auto-resizing the comment textarea while typing)
- `plone.formwidget.captcha`_ (for Captcha spam protection)
- `plone.formwidget.recaptcha`_ (for ReCaptcha spam protection)

.. _`collective.autoresizetextarea`: http://pypi.python.org/pypi/collective.autoresizetextarea
.. _`plone.formwidget.captcha`: http://pypi.python.org/pypi/plone.formwidget.captcha
.. _`plone.formwidget.recaptcha`: http://pypi.python.org/pypi/plone.formwidget.recaptcha


Credits
=======

- Timo Stollenwerk
- Martin Aspeli

Many thanks to:

- Jon Stahl (for acting as "the customer" during GSoC)
- David Glick (for technical expertise and advice during GSoC)
- Lennart Regebro (for writing the portal_discussion tool and initial unit tests)
- Carsten Senger (for fixing the comment z3c.form form and pizza)
- Hanno Schlichting (for making p.a.d work with Zope 2.12)
- Alan Hoey (for providing fixes)
- Maik Röder (for providing and setting up a buildbot)
