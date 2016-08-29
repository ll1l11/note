ubuntu16.04升级后, pip如下报错：

.. code:: bash

    $ pip
    Traceback (most recent call last):
      File "/usr/local/bin/pip", line 5, in <module>
        from pkg_resources import load_entry_point
    ImportError: No module named 'pkg_resources'

解决方式： http://stackoverflow.com/questions/18546321/how-do-you-uninstall-the-package-manager-pip-if-installed-from-source

.. code:: bash

    easy_install -m pip
