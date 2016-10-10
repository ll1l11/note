=============
vim的一些使用
=============

.. contents::

---------------------
insert custom content
---------------------

- ~/.vim/plugin/insert-custom-content.vim

    .. code:: vim

        function! PyFirstLine()
            " ~/.vim/plugin/in... is the path to the template file
            " r~/.vim/plugin/insert-custom-content.vim
            call append(0, "# -*- coding: utf-8 -*-")
        endfunction

        nmap <C-i> :call PyFirstLine()<CR>



--------------
copy and paste
--------------

- `How to make vim paste from (and copy to) system's clipboard? <http://stackoverflow.com/questions/11489428/how-to-make-vim-paste-from-and-copy-to-systems-clipboard/11489440#11489440>`_

- `mac ubuntu同步vim粘贴板 <http://www.jianshu.com/p/2436a05e180e>`_
