To run this project you first need to have the following applications installed:
	1. PHP: https://www.php.net/downloads.php
	2. Xampp: https://www.apachefriends.org/
	3. Composer: https://getcomposer.org/download/

1. Open Xampp and start Apache and MySQL services
2. Once composer is installed open git bash or cmd in the project location and run the following command: composer update
	This should generate a file called 'vendor'
3. Next run this command: php artisan key:generate
4. Open  http://localhost/phpmyadmin   and create a new database. Name it whatever you want.
5. Rename .env.example file to just .env 
6. Open  .env  file, find and insert databse name   DB_DATABASE='name of the database created' 
  Don't forget to save.
7. Run: php artisan migrate
8. Run: php artisan serve   to start the server and open it.
