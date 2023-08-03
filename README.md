# Gerador de CRUDs para laravel
Gerador de CRUDs para laravel com suporte a API

Gerador de CRUDs para Laravel

Com suporte ao laravel 9 e 10

https://github.com/sohelamin/crud-generator

composer require appzcoder/crud-generator --dev

php artisan vendor:publish --provider="Appzcoder\CrudGenerator\CrudGeneratorServiceProvider"

Example

php artisan crud:generate Posts --fields='title#string; email#string;' --controller-namespace=App\\Http\\Controllers --form-helper=html

## Adjusts routes in /routes/web:

Route::resource('admin/products', 'App\Http\Controllers\Admin\ProductsController');

php artisan route:clear

php artisan migrate

php artisan serve

http://127.0.0.1:8000/posts

## In case of problem run:

php artisan route:list

## [Tutorial para API](api-tutorial.md) (in pt-br)
