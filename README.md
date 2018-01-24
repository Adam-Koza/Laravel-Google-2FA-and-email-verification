# Laravel-with-Google-2FA-and-email-verification
Laravel 5.5 with Google Two-Factor Authentication and E-mail Verification

This project was constructed following these tutorials:
Email verification: https://itsolutionstuff.com/post/laravel-5-email-verification-with-activation-code-exampleexample.html
Google 2FA: https://www.5balloons.info/two-factor-authentication-google2fa-laravel-5/

# Verification email is sent to user upon registration:
![Send Email Verification](https://i.imgur.com/wgbyrzi.png)

# Can't login without verification:
![Can't login without verification](https://i.imgur.com/zpvagwF.png)

# Find 2-Factor Authentication setting in the User drop down menu:
![drop down menu](https://i.imgur.com/XnsLj7w.png)

# Enable 2-Factor Authentication:
![Enable 2-Factor](https://i.imgur.com/mx7rk2l.png)

# User is prompted for OTP when logging in:
![User is prompted](https://i.imgur.com/6baIQqV.png)

# Disable 2-Factor:
![Disable 2-Factor](https://i.imgur.com/IZAiWOE.png)



# Install:

- Clone this project.
- Install composer: "curl -sS https://getcomposer.org/installer | sudo php -- --install-dir=/usr/local/bin --filename=composer"
- Go to the folder application using cd.
- Run "composer install" on your cmd or terminal.
- Copy .env.example file to .env on root folder. You can type copy .env.example .env if using command prompt Windows or "cp .env.example .env" if using terminal Ubuntu.
- Open your .env file and change the database name (DB_DATABASE) to whatever you have, username (DB_USERNAME) and password (DB_PASSWORD) field correspond to your configuration. By default, username is root and you can leave password field empty. (This is for Xampp). By default, username is root and password is also root. (This is for Lamp).
- In your .env file enter your SMTP information for sending mail.
- in config/mail.php, on line 59 change hello@example.com to your mailing from address and replace "Your Name Here" with your name.
- in app/Http/Controllers/PasswordSecurityController.php on line 28, replace "COMPANY NAME" with your website, this is what the token will be named on user's google authenticators.
- Run php artisan key:generate
- Run php artisan migrate
- Run php artisan serve
- Go to localhost:8000


