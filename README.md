OASISWORK FORK DISCLAIMER
==========================

This is a temporary fork, just to be used with oazim lib, waiting for upstream
pyisimplesoap to include changes, do not rely on it. It will be destroyed then.

Upstream is https://github.com/pysimplesoap/pysimplesoap

This fork includes two patches (and that's all) :

* http://code.google.com/p/pysimplesoap/issues/detail?id=115#c2
* http://code.google.com/p/pysimplesoap/issues/detail?id=89#c2

Below is the original README

Features
========

This fork has the following features:

* Corrected support for multiple SOAP ports/bindings
* Support for both `import` and `include` stanzas in WSDL
* Support for a WSDL base directory to deal with relative pathnames in import/include stanzas
* Somewhat saner traceing/logging (traces now go to log.debug(), which you can handle per module)
* Somewhat more readable logic (by removing a bunch of helpers to a separate file)


Testing
=======

Using Python 2.7+:

    python -m unittest discover

Using older Python versions:

    python -m unittest tests/suite.py

Code coverage:

    sudo pip install coverage
    coverage run tests/suite.py
    coverage report -m
    coverage html


