.. code-block::

    server {
        listen 80;
        listen 443 ssl;
        server_name you-domain.com;

        location / {
            proxy_pass http://localhost:8080;

            proxy_set_header   host             $host;

            add_header 'access-control-allow-origin' '$http_origin';
            add_header 'access-control-allow-credentials' 'true';
            add_header 'access-control-allow-methods' 'get, post, put, patch, options';
            add_header 'access-control-allow-headers' 'dnt,x-customheader,keep-alive,user-agent,x-requested-with,if-modified-since,cache-control,content-type,authorization';

        }

    }
