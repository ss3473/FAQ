# 

To run the FAQ Final project:
1. Git clone https://github.com/ss3473/FAQ.git
2. cd into FAQ and run composer install
3. cp .env.example to .env
4. setup database / with sqlite or other (https://laravel.com/docs/5.6/database)
5. Run: php artisan migrate
6. Run: unit tests: phpunit
7. Run: seeds php artisan migrate:refresh --seed