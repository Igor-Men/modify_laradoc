###Dockerize php Laravel application with stack php mysql apache2
this repo is modify from https://github.com/laradock/laradock

#Usage
###clone this repo to your root project folder, and follow by steps:

###build environment   
`docker-compose up -d apache2 mysql`

###look processec and pick what you need
`docker ps -a`

###install php dependecies and run seeds
`docker exec -ti <container workspase id/name> composer install`  
`docker exec -ti <container workspase id/name> php artisan migrate --seed`
