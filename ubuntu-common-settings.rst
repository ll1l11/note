========================
 ubuntu日常使用的一些设置
========================

.. contents::

-------------------
 Set Default Editor
-------------------

.. code:: bash

    select-editor

or:

.. code:: bash

    update-alternatives --config editor

-----------------------------
 Set Up Time Synchronization
-----------------------------

.. code:: bash

    sudo ntpdate cn.pool.ntp.org

----------------
sudo no password
----------------

- `How to run sudo command with no password? <http://askubuntu.com/questions/192050/how-to-run-sudo-command-with-no-password/443071#443071>`_ 

也可以执行::

    sudo visudo

在最后一行添加::

    <your username>  ALL=(ALL) NOPASSWD:ALL
