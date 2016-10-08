===========
openssh设置
===========

.. contents::

-----------------
authorized_keys
-----------------

:location: ~/.ssh/authorized_keys


-------
config
-------

.. code::

    ## override as per host ##
    Host server1
        HostName 192.168.1.1
        User server1-user
        Port 9999
        IdentityFile ~/.ssh/ganma_rsa

    ## default for all ##
    Host *
        TCPKeepAlive yes
        ServerAliveInterval 30
        ServerAliveCountMax 10
        User ubuntu
