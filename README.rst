urllib3
=======

.. image:: https://travis-ci.org/urllib3/urllib3.svg?branch=master
        :alt: Build status on Travis
        :target: https://travis-ci.org/urllib3/urllib3

.. image:: https://img.shields.io/appveyor/ci/urllib3/urllib3/master.svg
        :alt: Build status on AppVeyor
        :target: https://ci.appveyor.com/project/urllib3/urllib3

.. image:: https://readthedocs.org/projects/urllib3/badge/?version=latest
        :alt: Documentation Status
        :target: https://urllib3.readthedocs.io/en/latest/

.. image:: https://img.shields.io/codecov/c/github/urllib3/urllib3.svg
        :alt: Coverage Status
        :target: https://codecov.io/gh/urllib3/urllib3

.. image:: https://img.shields.io/pypi/v/urllib3.svg?maxAge=86400
        :alt: PyPI version
        :target: https://pypi.org/project/urllib3/

.. image:: https://badges.gitter.im/python-urllib3/Lobby.svg
        :alt: Gitter
        :target: https://gitter.im/python-urllib3/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge

.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black

urllib3 is a powerful, *sanity-friendly* HTTP client for Python. Much of the
Python ecosystem already uses urllib3 and you should too.
urllib3 brings many critical features that are missing from the Python
standard libraries:

*Currently not supporting SOCKS proxies, pyOpenSSL and SecureTransport.*

- Thread safety.
- Connection pooling.
- Client-side SSL/TLS verification.
- File uploads with multipart encoding.
- Helpers for retrying requests and dealing with HTTP redirects.
- Support for gzip, deflate, and brotli encoding.
- Proxy support for HTTP and SOCKS.
- 100% test coverage.

urllib3 is powerful and easy to use::

    >>> import urllib3
    >>> http = urllib3.PoolManager()
    >>> r = http.request('GET', 'http://httpbin.org/robots.txt')
    >>> r.status
    200
    >>> r.data
    'User-agent: *\nDisallow: /deny\n'


Installing
----------

urllib3 can be installed with `pip <https://pip.pypa.io>`_::

    $ pip install urllib3

Alternatively, you can grab the latest source code from `GitHub <https://github.com/urllib3/urllib3>`_::

    $ git clone git://github.com/urllib3/urllib3.git
    $ python setup.py install


Documentation
-------------

urllib3 has usage and reference documentation at `urllib3.readthedocs.io <https://urllib3.readthedocs.io>`_.


Contributing
------------

urllib3 happily accepts contributions. Please see our
`contributing documentation <https://urllib3.readthedocs.io/en/latest/contributing.html>`_
for some tips on getting started.


Maintainers
-----------

- `@sethmlarson <https://github.com/sethmlarson>`_ (Seth M. Larson)
- `@pquentin <https://github.com/pquentin>`_ (Quentin Pradet)
- `@theacodes <https://github.com/theacodes>`_ (Thea Flowers)
- `@haikuginger <https://github.com/haikuginger>`_ (Jess Shapiro)
- `@lukasa <https://github.com/lukasa>`_ (Cory Benfield)
- `@sigmavirus24 <https://github.com/sigmavirus24>`_ (Ian Cordasco)
- `@shazow <https://github.com/shazow>`_ (Andrey Petrov)

👋


Sponsorship
-----------

If your company benefits from this library, please consider `sponsoring its
development <https://urllib3.readthedocs.io/en/latest/contributing.html#sponsorship-project-grants>`_.

Sponsors include:

- Abbott (2018-2019), sponsored `@sethmlarson <https://github.com/sethmlarson>`_'s work on urllib3.
- Google Cloud Platform (2018-2019), sponsored `@theacodes <https://github.com/theacodes>`_'s work on urllib3.
- Akamai (2017-2018), sponsored `@haikuginger <https://github.com/haikuginger>`_'s work on urllib3
- Hewlett Packard Enterprise (2016-2017), sponsored `@Lukasa’s <https://github.com/Lukasa>`_ work on urllib3.
