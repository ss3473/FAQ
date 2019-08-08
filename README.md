# 

To run the FAQ Final project:
1. Git clone https://github.com/ss3473/FAQ.git
2. cd into FAQ and run composer install
3. cp .env.example to .env
4. setup database / with sqlite or other (https://laravel.com/docs/5.6/database)
5. Run: php artisan migrate
6. Run: unit tests: phpunit
7. Run: seeds php artisan migrate:refresh --seed

Final Project Update
Heroku Link: (http://is601finalfaqfeature.herokuapp.com/home)
Github Link: (https://github.com/ss3473/FAQ)
EPIC Feature Added: (https://developers.google.com/recaptcha/docs/v3)
Steps to integrate new feature:
1. Register your site and domain on the following google recaptcha site:
(https://www.google.com/recaptcha/admin/)
    Add Label
    Add herokuapp.com in your domain
    Click on Save and then proceed to the next steps.
2. You will receive Site and Secret Key that you'll need to update into your code.
3. Run composer require biscolab/laravel-recaptcha:^3.0
4. Modify your code, validate locally and then on heroku. Please make sure to include herokuapp.com in the accepted list of domains for google recaptcha.

USER STORIES
1. Google Recaptcha v3 is the latest API provided by google that allows you to detect abusive traffic on your site without user interaction.
Using this latest tool I am able to launch the login page on my laravel site and see the Recaptcha v3 on the bottom right corner. 

2. On the Laravel registration page for new users google recaptcha v3 runs seamlessly as the user registers and authenticates to the site. The recaptcha v3 api stays running in the bottom right corner and does not create any issues for user registration. 
