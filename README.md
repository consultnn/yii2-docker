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
Rename example nginx config to mysite.confgit 
Run
~~~
docker-compose up -d
~~~
For executing commands inside docker container run
~~~
docker-compose run php {command}
~~~
