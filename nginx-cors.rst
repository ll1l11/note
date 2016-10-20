================
nginx cors的配置
================

.. contents::


------------
all request
------------


.. code::

    location / {
        proxy_pass http://card-test;

        proxy_set_header   Host             $host;

        add_header 'Access-Control-Allow-Origin' '$http_origin';
        add_header 'Access-Control-Allow-Credentials' 'true';
        add_header 'Access-Control-Allow-Methods' 'GET, POST, PUT, PATCH, OPTIONS';
        add_header 'Access-Control-Allow-Headers' 'DNT,X-CustomHeader,Keep-Alive,User-Agent,X-Requested-With,If-Modified-Since,Cache-Control,Content-Type';

    }


--------------------
multiple domain(map)
--------------------

- `slbmeh/nginx-cors.conf <https://gist.github.com/slbmeh/6e2dbc1218a0be0d7ae2>`_
