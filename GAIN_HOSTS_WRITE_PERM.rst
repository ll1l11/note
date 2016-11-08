How to grant your account write permissions to file hosts
=========================================================

https://code.google.com/archive/p/fire-hostadmin/wikis/GAIN_HOSTS_WRITE_PERM.wiki

Introduction
-------------

Grant your account write permission to hosts file thus HostAdmin could change host while Firefox running

Windows Vista/7
---------------

- To Users group

.. code-block::

    cacls %windir%/system32/drivers/etc/hosts /E /G Users:W

- Custom User account

.. code-block::

    cacls %windir%/system32/drivers/etc/hosts /E /G "User Account Name":W

Linux (Ubuntu Fedora ...)
--------------------------

.. code-block::

    sudo chmod og+w /etc/hosts

Mac OS X
---------

.. code-block::

    sudo chmod og+w /etc/hosts
