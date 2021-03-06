
======
slimer
======


``slimer`` is an object available automatically in scripts.



.. _slimer-clearHttpAuth:

clearHttpAuth()
-----------------------------------------

It clears all HTTP authentication that have been made. Then, when
a webpage needs an HTTP auth, username and password will be asked again.

See :doc:`doc about http authentication with SlimerJS <../manual/http-authentication>`.


.. _slimer-exit:

exit()
-----------------------------------------


It stops the script and SlimerJS exit.

It accepts an optional exit code but it is ignored
because of a limitation in Firefox/XulRunner.

.. code-block:: javascript

    slimer.exit();


.. _slimer-version:

version
-----------------------------------------

Contain the version of SlimerJS (read-only). This is an object
containing three properties, ``major``, ``minor``, ``patch``:

.. code-block:: javascript

    var v = slimer.version;
    console.log('version: ' + v.major + '.' + v.minor + '.' + v.patch);

