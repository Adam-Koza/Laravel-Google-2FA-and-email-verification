# Laravel-with-Google-2FA-and-email-verification
Laravel with Google 2FA and email verification

Project was constructed following these tutorials:

Email verification: https://itsolutionstuff.com/post/laravel-5-email-verification-with-activation-code-exampleexample.html

Google 2FA: https://www.5balloons.info/two-factor-authentication-google2fa-laravel-5/

# Install:

- Clone your project.
- Install composer: "curl -sS https://getcomposer.org/installer | sudo php -- --install-dir=/usr/local/bin --filename=composer"
- Go to the folder application using cd.
- Run "composer install" on your cmd or terminal.
- Copy .env.example file to .env on root folder. You can type copy .env.example .env if using command prompt Windows or "cp .env.example .env" if using terminal Ubuntu.
- Open your .env file and change the database name (DB_DATABASE) to whatever you have, username (DB_USERNAME) and password (DB_PASSWORD) field correspond to your configuration.
- By default, username is root and you can leave password field empty. (This is for Xampp).
- By default, username is root and password is also root. (This is for Lamp).
- Run php artisan key:generate
- Run php artisan migrate
- Run php artisan serve
- Go to localhost:8000


