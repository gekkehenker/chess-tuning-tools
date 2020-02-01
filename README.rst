==================
Chess Tuning Tools
==================


.. image:: https://img.shields.io/pypi/v/chess-tuning-tools.svg
        :target: https://pypi.python.org/pypi/chess-tuning-tools

.. image:: https://img.shields.io/travis/kiudee/chess-tuning-tools.svg
        :target: https://travis-ci.org/kiudee/chess-tuning-tools

.. image:: https://readthedocs.org/projects/chess-tuning-tools/badge/?version=latest
        :target: https://chess-tuning-tools.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status




A collection of tools for local and distributed tuning of chess engines.


* Free software: Apache Software License 2.0
* Documentation: https://chess-tuning-tools.readthedocs.io.


Features
--------

* TODO


Starting the tuning client
--------------------------
In order to be able to start the tuning client, first create a python
environment and install chess-tuning-tools by typing::

   pip install chess-tuning-tools

Furthermore, you need to have `cutechess-cli <https://github.com/cutechess/cutechess>`_
in the path. The tuning client will use it to run matches.

Then after extracting the current .zip package into another folder, make sure that you have the following directory
structure::

   folder/
   |---- networks/
   |     |---- 58613
   |     |---- other networks
   |---- openings/
   |     |---- ...
   |     |---- openings-6ply-1000.pgn
   |     |---- ...
   |---- dbconfig.json
   |---- lc0[.exe]
   |---- sf[.exe]

Finally, the tuning client can be started as follows::

   cd path/to/folder
   tune run-client dbconfig.json


Credits
-------

This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage