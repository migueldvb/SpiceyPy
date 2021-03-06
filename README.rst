SpiceyPy
========

SpiceyPy is a Python wrapper for the NAIF C SPICE Toolkit (N66), written using ctypes.

+------------------------------------------------+---------------------+--------------------------+-------------------+------------+--------------+
| Continuous Integration                         | Code Coverage       | Docs                     | Chat              | Citation   |  Code Style  |
+================================================+=====================+==========================+===================+============+==============+
| |Travis Build Status| |Windows Build Status|   | |Coverage Status|   | |Documentation Status|   | |Join the chat|   | |Citation| |  |Black|     |
+------------------------------------------------+---------------------+--------------------------+-------------------+------------+--------------+

.. |Travis Build Status| image:: https://img.shields.io/travis/Originate/tertestrial-server/master.svg?logo=travis
   :target: https://travis-ci.org/AndrewAnnex/SpiceyPy
.. |Windows Build Status| image:: https://ci.appveyor.com/api/projects/status/wly0q2cwy33ffura/branch/master?svg=true
   :target: https://ci.appveyor.com/project/AndrewAnnex/spiceypy/
.. |Coverage Status| image:: https://coveralls.io/repos/github/AndrewAnnex/SpiceyPy/badge.svg?branch=master
   :target: https://coveralls.io/github/AndrewAnnex/SpiceyPy?branch=master
.. |Documentation Status| image:: https://readthedocs.org/projects/spiceypy/badge/?version=master
   :target: http://spiceypy.readthedocs.org/en/master/
.. |Join the chat| image:: https://badges.gitter.im/Join%20Chat.svg
   :target: https://gitter.im/AndrewAnnex/SpiceyPy?utm_source=badge
.. |Citation| image:: https://zenodo.org/badge/16987/AndrewAnnex/SpiceyPy.svg
   :target: https://zenodo.org/badge/latestdoi/16987/AndrewAnnex/SpiceyPy
.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg 
   :target: https://github.com/psf/black


Introduction
------------

SpiceyPy is a python wrapper for the `SPICE Toolkit <https://naif.jpl.nasa.gov/naif/>`__.
SPICE is an essential tool for scientists and engineers alike in the planetary
science field for Solar System Geometry. Please visit the NAIF website for more details about SPICE.

*IMPORTANT*: I have no current affiliation with NASA, NAIF, or JPL. The
code is provided "as is", use at your own risk. However, the NAIF now distributes python "lessons" that use SpiceyPy as the python to spice interface.

Citing SpiceyPy
---------------

If you are publishing work that uses SpiceyPy, please cite
SpiceyPy and the SPICE toolkit. The citation information
for SPICE can be found on the NAIF website. To cite SpiceyPy please
utilize the zenodo DOI badge at the top of this readme. To cite information 
about SpiceyPy, usership, and how it works please cite my 2017 abstract, available with citation info at : `<https://ui.adsabs.harvard.edu/#abs/2017LPICo1986.7081A>`__.

Installation
------------

+----------------+-------------------+
| PyPI           | Conda Forge       |
+================+===================+
| |PyPI|         | |Conda Version|   |
+----------------+-------------------+

.. |PyPI| image:: https://img.shields.io/pypi/v/spiceypy.svg
   :target: https://pypi.org/project/spiceypy/
.. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/spiceypy.svg
   :target: https://anaconda.org/conda-forge/spiceypy

SpiceyPy can be installed using pip by running:
``pip install spiceypy``

Anaconda users should use the conda-forge distribution of SpiceyPy by running:

``conda config --add channels conda-forge``

``conda install spiceypy``

If you wish to install spiceypy from source first download or clone the project. Then run ``python setup.py install``.
To uninstall run ``pip uninstall spiceypy``.

Documentation
-------------

The SpiceyPy docs are available at:
`spiceypy.readthedocs.org <http://spiceypy.readthedocs.org>`__.
The documentation for SpiceyPy is intentionally abridged so as to utilize the excellent `documentation provided by the
NAIF. <https://naif.jpl.nasa.gov/pub/naif/toolkit_docs/C/index.html>`__
Please refer to C and IDL documentation available on the NAIF website
for in-depth explanations. Each function docstring has a link to the
corresponding C function in the NAIF docs at a minimum.
SpiceyPy documentation contains the NAIF authored `Lessons <https://spiceypy.readthedocs.io/en/master/lessonindex.html>`__ for step-by-step tutorials with code examples. 

How to Help
-----------

Feedback is always welcomed, if you discover that a function is not working as expected,
submit an issue detailing how to reproduce the problem. If you utilize SpiceyPy frequently 
please consider contributing to the project by citing me using the zenodo DOI above.

Known Working Environments:
---------------------------

SpicyPy is compatible with modern Linux, Mac, and Windows
environments. Since the package is a wrapper, any environment not
supported by the NAIF is similarly not supported by SpiceyPy.
If you run into issues with your system please submit an issue with details. 
Please note that support for Python minor versions are generally phased out 
as newer versions are released. 

- OS: OS X, Linux, Windows
- CPU: 64bit only!
- Python 3.6, 3.7, 3.8

* Support for Python 2.7 ended with version 2.3.2 January 2020 *

Acknowledgements
----------------

`DaRasch <https://github.com/DaRasch>`__ wrote spiceminer, which I
looked at to get SpiceCells working, thanks!

