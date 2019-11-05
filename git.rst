显示分之名
----------

https://github.com/jimeh/git-aware-prompt

`zsh下的自动补全 <https://github.com/github/hub/tree/master/etc>`_

使用代理
----------

.. code-block::

    git config --global http.proxy socks5://127.0.0.1:1080
    git config --global http.proxy http://127.0.0.1:8888

只是github使用代理
------------------

.. code-block:: sh

    git config --global http.https://github.com.proxy socks5://127.0.0.1:1080


git on the server
-------------------

文档:
https://git-scm.com/book/en/v2/Git-on-the-Server-Setting-Up-the-Server

设置方式::

    $ cd ~/git-repositories
    $ mkdir project.git
    $ cd project.git
    $ git init --bare
    Initialized empty Git repository in /srv/git/project.git/

对应的地址::

    git@gitserver:git-repositories/project.git


如果配置了GIR_DIR和GIR_WORK_TREE, 如果执行git init --bare则需要(`<https://stackoverflow.com/a/31802682/7403042>`_)::

    env -u GIT_WORK_TREE git init --bare


