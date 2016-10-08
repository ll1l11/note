=================
 python settings
=================

.. contents::

-----------------------------------------
 make sure install packages to virtualenv
-----------------------------------------

参考: http://docs.python-guide.org/en/latest/dev/pip-virtualenv/

.. code:: bash

    export PIP_REQUIRE_VIRTUALENV=true


---------
pip.conf
---------

:location: ~/.pip/pip.conf

.. code::

    [global]
    index-url = https://pypi.doubanio.com/simple
    trusted-host = pypi.doubanio.com

    ; [install]
    ; ignore-installed = true
    ; no-cache-dir = off
