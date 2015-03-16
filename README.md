Docker-compose config for Yii 2 Application Template
===================================
Yii 2 docker is a configuration for easy deployment of yii2 template application.

REQUIREMENTS
------------

Docker and Docker compose

INSTALLATION
------------
1. Clone this repository. 
~~~
git clone http://github.com/sokrat/yii2-docker.git app
~~~
2. Clone yii 2 application.
~~~
git clone https://github.com/yiisoft/yii2-app-advanced.git app/project
or
git clone https://github.com/yiisoft/yii2-app-basic.git app/project
~~~
3. Remove ".example" from nginx configuration example filename (docker/nginx/conf.d).
USING
------
For executing commands inside docker container run
~~~
docker-compose run {service} {command}
~~~
For example:
~~~
docker-compose run php composer install
docker-compose run php /www/init
~~~

Start docker containers.
~~~
docker-compose up -d
~~~
NOTE: for composer use --prefer-dist options, git not installed in php container.
After start check http://127.0.0.1:8090