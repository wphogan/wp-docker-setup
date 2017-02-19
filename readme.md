#Basic WordPress / PhpMyAdmin / MariaDB Docker setup 

### https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-and-phpmyadmin-with-docker-compose-on-ubuntu-14-04

### Commands:
`docker-compose stop`
`docker-compose up -d`

Kill all containers:
`docker kill $(docker ps -q)`

Remove all containers:
`docker rm $(docker ps -a -q)`

Remove all docker images: 
` docker rmi $(docker images -q)`

Show running containers:
`docker ps`

Show all containers:
`docker ps -a`

Enter a container:
`docker exec -it my-app-container-id bash`

Note: for wp-cli to work, must have wp-su.sh file in the root dir of Dockerfile (local-side, not docker-side)