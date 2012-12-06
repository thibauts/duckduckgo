duckduckgo.py
=============

duckduckgo.py is a simple python module to scrape the duckduckgo search results. The install script will also make available a ddg command line utility that can be conveniently used in a shell pipeline.

A word of warning
-----------------

This code is intended as a demonstration and, as all scraping utilities, should be used with great caution. By default the code will pause a few milliseconds each time it yields a result to avoid overloading the DDG servers.

Usage
-----

It can be used as a python module

.. code-block:: pycon

  >>> import duckduckgo
  >>> for link in duckduckgo.search('duckduckgo', max_results=10):
  ...     print link
  ...
  https://duckduckgo.com/
  https://en.wikipedia.org/wiki/DuckDuckGo
  https://duckduckgo.com/about.html
  [...]


Or as a command line tool

.. code-block:: bash

  $ ddg -n 10 duckduckgo


Installation
------------

.. code-block:: bash
  $ python setup.py install



