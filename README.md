[![Build Status](https://travis-ci.org/hoyvoy/laravel-cross-database-subqueries.svg?branch=master)](https://travis-ci.org/hoyvoy/laravel-cross-database-subqueries) [![Codacy Badge](https://api.codacy.com/project/badge/Grade/5ef152edf13d4440a9ccacf942bbecf9)](https://www.codacy.com/app/mario-hoyvoy/laravel-cross-database-subqueries?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=hoyvoy/laravel-cross-database-subqueries&amp;utm_campaign=Badge_Grade) [![StyleCI](https://styleci.io/repos/120466504/shield?branch=master)](https://styleci.io/repos/120466504)

# Laravel Cross database subqueries
Eloquent cross database compatibility in subqueries.

# Why do I need it?
### To use the following Eloquent methods cross databases:
* has
* whereHas
* doesntHave 
* whereDoesntHave
* withCount (except using prefixes)

# Installation
Install with composer
~~~
composer require hoyvoy/laravel-cross-database-subqueries
~~~

From Laravel 5.5 onwards, it's possible to take advantage of auto-discovery of the service provider.
For Laravel versions before 5.5, you must register the service provider in your config/app.php

~~~
Hoyvoy\CrossDatabase\CrossDatabaseServiceProvider::class,
~~~

# Usage
In your `Models` extends from:
* Hoyvoy\CrossDatabase\Eloquent\Model

# Supported PHP Versions
* \>=7.0

# Supported Databases
* MySQL
* PostgreSQL
* SQL Server

# Issues & Contributing
If you find an issue please report it or contribute by submitting a pull request.