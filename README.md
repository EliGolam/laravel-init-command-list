# laravel-init-command-list
How to start Laravel Projects

## Windows

### Laravel 7

#### Create brand new project

1. composer create-project --prefer-dist laravel/laravel:^7.0 new-project
2. npm i
3. git init
4. Open "webpack.mix.js" and add "mix.browserSync('127.0.0.1:8000')"
5. npm install browser-sync browser-sync-webpack-plugin
6. php artisan serve
7. npm run watch

#### Clone project from remote repo

1. composer install
2. cp .env.example .env (copy .env.example as .env file)
3. php artisan key:generate
4. Create necessary databases
5. Add .env credentials
6. php artisan config:cache
7. Migrate and Seed database (php artisan migrate, php artisan db:seed --class=UsersTableSeeder)
8. npm i
9. php artisan serve
10. npm run watch

#### Optional Elements

##### Faker

1. composer remove --dev fzaninotto/faker
2. composer require --dev fakerphp/faker

##### Node 18+ bug 
if it gives error, it may be because node 18 is being used. 
* npm install cross-env
* "development": "cross-env NODE_ENV=development NODE_OPTIONS='**--openssl-legacy-provider**' ..."
