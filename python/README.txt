blosc: a Python package that wraps the Blosc compressor
=======================================================

Blosc is a high performance compressor optimized for binary data.  It
has been designed to transmit data to the processor cache faster than
the traditional, non-compressed, direct memory fetch approach via a
memcpy() OS call.

The functions in this package allow compression and decompression
using the Blosc library (http://blosc.pytables.org).

Building
--------

Assuiming that you have a C compiler installed, do:

$ python setup.py build_ext --inplace

Testing
-------

After compiling, you can quickly check that the package is sane by
running:

$ PYTHONPATH=.   (or "set PYTHONPATH=." on Win)
$ export PYTHONPATH=.  (not needed on Win)
$ python blosc/toplevel.py

Installing
----------

Install it as a typical Python package:

$ python setup.py install

Documentation
-------------

Please refer to docstrings.  Start by the main package:

>>> import blosc
>>> help(blosc)

and ask for more docstrings in the referenced functions.
