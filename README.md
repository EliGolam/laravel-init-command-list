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

* composer install
* cp .env.example .env (copy .env.example as .env file)
* php artisan key:generate
* Create necessary databases
* Add .env credentials
* Migrate and Seed database (php artisan migrate, php artisan db:seed --class=UsersTableSeeder)
* npm i



if it gives error, it may be because node 18 is being used. 
* npm install cross-env
* "development": "cross-env NODE_ENV=development NODE_OPTIONS='**--openssl-legacy-provider**' ..."
