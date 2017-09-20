显示分之名
----------

https://github.com/jimeh/git-aware-prompt

使用代理

.. code-block::

    [http]
      proxy = socks5://127.0.0.1:1080
    [https]
      proxy = socks5://127.0.0.1:1080


只能在virtualenv中安装package, 在.bashrc中添加::

    # call pip only in virtualenv
    export PIP_REQUIRE_VIRTUALENV=true
    
    
git on the server
------------------

文档:
https://git-scm.com/book/en/v2/Git-on-the-Server-Setting-Up-the-Server

设置方式::

    $ cd ~/git-repositories
    $ mkdir project.git
    $ cd project.git
    $ git init --bare
    Initialized empty Git repository in /srv/git/project.git/

对应的地址::

    git@gitserver:~/git-repositories/project.git
