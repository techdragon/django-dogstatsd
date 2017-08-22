========
Overview
========

.. start-badges

.. list-table::
    :stub-columns: 1

    * - docs
      - |docs|
    * - tests
      - | |travis| |appveyor| |requires|
        | |codecov|
        | |landscape| |scrutinizer| |codeclimate|
    * - package
      - | |version| |wheel| |supported-versions| |supported-implementations|
        | |commits-since|

.. |docs| image:: https://readthedocs.org/projects/django-dogstatsd/badge/?style=flat
    :target: https://readthedocs.org/projects/django-dogstatsd
    :alt: Documentation Status

.. |travis| image:: https://travis-ci.org/techdragon/django-dogstatsd.svg?branch=master
    :alt: Travis-CI Build Status
    :target: https://travis-ci.org/techdragon/django-dogstatsd

.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/github/techdragon/django-dogstatsd?branch=master&svg=true
    :alt: AppVeyor Build Status
    :target: https://ci.appveyor.com/project/techdragon/django-dogstatsd

.. |requires| image:: https://requires.io/github/techdragon/django-dogstatsd/requirements.svg?branch=master
    :alt: Requirements Status
    :target: https://requires.io/github/techdragon/django-dogstatsd/requirements/?branch=master

.. |codecov| image:: https://codecov.io/github/techdragon/django-dogstatsd/coverage.svg?branch=master
    :alt: Coverage Status
    :target: https://codecov.io/github/techdragon/django-dogstatsd

.. |landscape| image:: https://landscape.io/github/techdragon/django-dogstatsd/master/landscape.svg?style=flat
    :target: https://landscape.io/github/techdragon/django-dogstatsd/master
    :alt: Code Quality Status

.. |codeclimate| image:: https://codeclimate.com/github/techdragon/django-dogstatsd/badges/gpa.svg
   :target: https://codeclimate.com/github/techdragon/django-dogstatsd
   :alt: CodeClimate Quality Status

.. |version| image:: https://img.shields.io/pypi/v/django-dogstatsd.svg
    :alt: PyPI Package latest release
    :target: https://pypi.python.org/pypi/django-dogstatsd

.. |commits-since| image:: https://img.shields.io/github/commits-since/techdragon/django-dogstatsd/v0.1.0.svg
    :alt: Commits since latest release
    :target: https://github.com/techdragon/django-dogstatsd/compare/v0.1.0...master

.. |wheel| image:: https://img.shields.io/pypi/wheel/django-dogstatsd.svg
    :alt: PyPI Wheel
    :target: https://pypi.python.org/pypi/django-dogstatsd

.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/django-dogstatsd.svg
    :alt: Supported versions
    :target: https://pypi.python.org/pypi/django-dogstatsd

.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/django-dogstatsd.svg
    :alt: Supported implementations
    :target: https://pypi.python.org/pypi/django-dogstatsd

.. |scrutinizer| image:: https://img.shields.io/scrutinizer/g/techdragon/django-dogstatsd/master.svg
    :alt: Scrutinizer Status
    :target: https://scrutinizer-ci.com/g/techdragon/django-dogstatsd/


.. end-badges

Django support for DataDog StatsD metrics.

* Free software: BSD license

Installation
============

::

    pip install django-dogstatsd

Documentation
=============

https://django-dogstatsd.readthedocs.io/

Development
===========

To run the all tests run::

    tox

Note, to combine the coverage data from all the tox environments run:

.. list-table::
    :widths: 10 90
    :stub-columns: 1

    - - Windows
      - ::

            set PYTEST_ADDOPTS=--cov-append
            tox

    - - Other
      - ::

            PYTEST_ADDOPTS=--cov-append tox
