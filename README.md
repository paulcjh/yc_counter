# yc_counter
Clone this repo and point nginx to the location of the directory. For example us this as your "default" in /etc/nginx/sites-enabled/default

```
        server {
        listen 80 default_server;
        listen [::]:80 default_server;
        server_name yc_counter.winning;       

        root /var/www/html;

        location / {
        alias /yc_counter/;
        }
        }
```
