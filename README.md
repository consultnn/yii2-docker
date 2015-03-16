Docker-compose config for Yii 2 Application Template
===================================
Yii 2 docker is a configuration for rapidly compose yii2 infrastructure.

REQUIREMENTS
------------

Docker and Docker compose

INSTALLATION
------------
Clone this repository. 
~~~
git clone http://github.com/sokrat/yii2-docker.git app
~~~
Clone yii 2 application to app directory with name "project"
Rename needed example nginx configuration to mysite.conf

USING
------
For executing commands inside docker container run
~~~
docker-compose run php {command}
~~~
Start docker containers 
~~~
docker-compose up -d
~~~
After start check http://127.0.0.1:8090