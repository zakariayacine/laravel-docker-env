# laravel-docker-env<br>
A docker compose how prepare an environement for your laravel application in 2 ligne<br>
To use it you need to: <br>
1 - install docker & docker compose <br>(find the version of your OS) <br>(i recomande to change the ip address and the password for mariadb)<br>
2 - copy the files in the directory of your choice<br>
3 - start the commandes : docker-compose build && docker-compose up -d<br>
4 - copy files of your laravel in .src/ or go in the php container and start install a new laravel project like this :<br>
  1 - "docker exec php php /var/www/html composer global require laravel/installer" or you can go in your container like so<br>
    * "docker exec -it php /bin/sh" you will be in the container and after that you can execute <br>"composer global require laravel/installer" or "php artisan" commands
  2 - change the .env file and add address and the username/password/dbname (that you made in the docker-compose)<br>
  3 - run "php artisan migrate" and you are done !!<br>
***PS : sorry for my englich i will make another readme file***<br>
