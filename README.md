#Requirements
•	PHP >= 7.1.3
•	OpenSSL PHP Extension
•	PDO PHP Extension
•	Mbstring PHP Extension
•	Tokenizer PHP Extension
•	XML PHP Extension
•	Ctype PHP Extension
•	JSON PHP Extension
•	Mysql server

How to run the application

#Set up the application database

Go to your terminal window and login to mysql
>mysql –u ‘yourusername’ –p’yourpassword’

Create the database
>CREATE DATABASE cytonn_app;

Create user
>CREATE USER ‘cytonn_app’@’localhost’ IDENTIFED BY ‘cytonn_app’;

Grant access to user
>GRANT ALL ON cytonn_app.* TO ‘cytonn_app’@’localhost’;

#Set up application
Open a new terminal window and navigate to the top level of your local repository

Run the following commands

composer install
composer artisan cache:clear
composer artisan config:cache
php artisan migrate:refresh –seed
php artisan serve

Run the application
Open browser and type localhost:8000


