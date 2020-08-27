Chaussette
==========

Chaussette is a WSGI server. The particularity of Chaussette is that
it can either bind a socket on a port like any other server does or
run against already opened sockets.

That makes Chaussette the best companion to run a WSGI or Django_ stack
under a process and socket manager, such as Circus_.

Since bjoern_ already support python 3, I trivially made the bjoern backend available for both python 2 and python 3.


Quick Start
-----------

Running:

.. code-block:: bash

   chaussette --backend bjoern bjoern-test.app.application

starts a very simple HTTP sample server on port 8080, and you should see "Damn!" with:

.. code-block:: bash

   curl localhost:8080

Links
-----

- The original repo is located at
  https://github.com/circus-tent/chaussette

.. _Circus: https://circus.readthedocs.io
.. _Django: https://docs.djangoproject.com
.. _bjoern: https://github.com/jonashaag/bjoern#why-its-cool

Changelog
---------

1.3.0 - 2020-08-27
~~~~~~~~~~~~~~~~~~

- Add bjoern backend for python 3.


