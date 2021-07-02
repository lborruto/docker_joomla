Please make sure to fix the permissions issues with `chmod o+rx *` to all folders.
----------------------------------------------------------------------------------------------------------------------

Use `docker-compose build` and `docker-compose up` for debugging.

Then use `docker-compose up -d` to run in background.

You should be able to get to `http://localhost/administrator` (or the ip of the virtual machine) and log in into Joomla :

user: admin
pass: secret

----------------------------------------------------------------------------------------------------------------------

`/database` contain the dockerfile for MariaDB, `/database/mysql` contain all the databases

`/nginx` contain the dockerfile for Nginx and `nginx.conf`, `/nginx/conf.d/` and `/nginx/site/` contain the `default.conf`

`/php-fpm` contain the dockerfile for PHP-FPM

`/joomla_logs` contain all the logs file for all of the containers

`/src` is the equivalent of `/var/www/html` for Nginx and Joomla

----------------------------------------------------------------------------------------------------------------------
