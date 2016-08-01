L5 Swagger
==========

Swagger 2.0 for Laravel >=5.1

This package is a wrapper of [Swagger-php](https://github.com/zircote/swagger-php) and [jensoleg/swagger-ui](https://github.com/jensoleg/swagger-ui) adapted to work with Laravel 5.

### Full credit to [DarkaOnLine/L5-Swagger](https://github.com/DarkaOnLine/L5-Swagger) for creating this package originally.

Installation
============

```php
    composer require "damian-nz/l5-swagger:~3.0"
```

- Open your `config/app.php` and add this line in `providers` section
```php
    L5Swagger\L5SwaggerServiceProvider::class
```

Configuration
============
- Run `l5-swagger:publish` to publish everything
- Run `l5-swagger:publish-config` to publish configs (`config/l5-swagger.php`)
- Run `l5-swagger:publish-assets` to publish swagger-ui to your public folder (`public/vendor/l5-swagger`)
- Run `l5-swagger:publish-views` to publish views (`resources/views/vendor/l5-swagger`)
- Run `l5-swagger:generate` to generate docs or set `generate_always` param to `true` in your config or .env file 

Swagger-php
======================
The actual Swagger spec is beyond the scope of this package. All L5-Swagger does is package up swagger-php and swagger-ui in a Laravel-friendly fashion, and tries to make it easy to serve. For info on how to use swagger-php [look here](http://zircote.com/swagger-php/). For good examples of swagger-php in action [look here](https://github.com/zircote/swagger-php/tree/master/Examples/petstore.swagger.io).
