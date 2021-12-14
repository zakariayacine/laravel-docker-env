# laravel-docker-env<br>
A docker compose how prepare an environement for your laravel application<br>
To use it you need to: <br>
<ul>
  <li>install docker & docker compose <br>(find the version of your OS) <br>(i recomande to change the ip address and the password for mariadb)</li>
  <li>copy the files in the directory of your choice</li>
  <li>start the commandes : docker-compose build && docker-compose up -d</li>
  <li>copy files of your laravel in .src/ or go in the php container and start install a new laravel project like this :</li>
  <ul>
    <li>"docker exec php php /var/www/html composer global require laravel/installer" or you can go in your container like so</li>
    <li>"docker exec -it php /bin/sh" you will be in the container</li>
    <li>and after that you can execute "composer global require laravel/installer" or "php artisan" commands</li>
    <li>change the .env file and add address and the username/password/dbname (that you made in the docker-compose)</li>
    <li>run "php artisan migrate" and you are done !! </li>
  </ul>
</ul>

<small><b>***PS : sorry for my englich i will make another readme file***</b><small>
