## We no longer maintain this repository. 

Docker-compose config for Yii 2 Application Template
===================================
Yii 2 docker is a configuration for easy deployment of yii2 template application.

REQUIREMENTS
------------

Docker and Docker compose

INSTALLATION
------------
Clone this repository and remove git files 
~~~
git clone http://github.com/consultnn/yii2-docker.git {your_app_name} && rm -rf {your_app_name}/.git
~~~
Change directory
~~~
cd {your_app_name}
~~~

Install yii 2 application.
~~~
docker-compose run --rm php composer create-project --prefer-dist yiisoft/yii2-app-advanced yii-application
or
docker-compose run --rm composer create-project --prefer-dist yiisoft/yii2-app-basic basict
~~~
Remove ".example" from nginx configuration example filename (docker/nginx/conf.d).

USING
------
For executing commands inside docker container run
~~~
docker-compose run --rm {service} {command}
or, if application already running
docker exec {service} {command}
~~~
For example:
~~~
docker-compose run php composer install
docker exec run php /init
~~~

Start docker containers
~~~
docker-compose up -d
~~~
NOTE: for composer use `--prefer-dist` options, git not installed in php container.

After start check http://127.0.0.1:8090
