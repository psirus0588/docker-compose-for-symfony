# Universal Docker containers: nginx+php-fpm+mariadb+postgres+redis+rabbitmq+elasticsearch+adminer+nodejs+yarn


List enabled PHP extensions:
Core, date, libxml, openssl, pcre, sqlite3, zlib, ctype, curl, dom, fileinfo, filter, ftp, hash, iconv, json, mbstring, SPL, PDO, pdo_sqlite, session, posix, readline, Reflection, standard, SimpleXML, Phar, tokenizer, xml, xmlreader, xmlwriter, mysqlnd, cgi, fcgi
amqp, pdo_mysql, redis, sockets, sodium


### Installation

```
git clone git@github.com:psirus0588/docker-compose-for-symfony.git

symfony new symfony_project

cd docker-compose-for-symfony

```

Start specific containers:
```
docker-compose up php-fpm nginx
```

Start all containers (php-fpm, nginx, redis, rabbitmq, elasticsearch, adminer, encore):
```
docker-compose up
```

Go to browser:
```
http://localhost
```




### How do I SSH into a running container
There is a docker exec command that can be used to connect to a container that is already running.

Use docker ps to get the name of the existing container
Use the command docker exec -it <container name> /bin/bash to get a bash shell in the container
Generically, use docker exec -it <container name> <command> to execute whatever command you specify in the container.