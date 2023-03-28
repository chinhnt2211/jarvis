### SETUP PROJECT 

## 1. Clone project:

## 2. Build project: 
   
``$ cd jarvis``

``$ cp .env.example .env``

Setup variable in file .env

|          Key          |        Value         |             Note              |
|:---------------------:|:--------------------:|:----------------------------:|
|     PROJECT_NAME      |        jarvis         |         name project        |
|         DEBUG         |    true or false     |   turn on or turn off debug  |
|  MYSQL_ROOT_PASSWORD  |         root         |  password of root user mysql |
|        PORT_DB        |         3306         |     port expose of mysql     |
|     PORT_ADMINER      |         9999         |    port expose of adminer    |
|     PORT_BACKEND      |         8000         |      port expose of API      |
|         PUID          | run command $ id -u  |      id of user login OS     |
|         PGID          | run command $ id -g  |     id of group login OS     |



``$ sudo docker compose build``

## 3. Run project: 
   
``$ sudo docker compose up -d``

## 4. Setup project:
``$ sudo docker exec -it jarvis_backend bash``

``$ composer install``

``$ php artisan key:generate``

``$ php artisan migrate``

## 5. Install a package in Laravel:
``$ sudo docker exec -it jarvis_backend bash``

``$ composer require [package_name]``

## 6. URL:

PhpMyAdmin: http://localhost:9999
<br>   
Web: http://localhost:8000