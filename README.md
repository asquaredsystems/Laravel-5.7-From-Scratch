[TOC]

# Laravel 5.7 From Scratch

## [The Laravel Sell](https://laracasts.com/series/laravel-from-scratch-2018/episodes/1)

> Presumably, if you're watching this series, 
you've already made the decision to embrace all that Laravel has to offer. 
However, if you're still on the fence, 
give me just a moment to sell you on 
why I believe Laravel is the best framework choice in the PHP world.

### Useful Website

- [Laravel - The PHP Framework For Web Artisans](https://laravel.com/)

- [Laracasts](https://laracasts.com/)

- [Laravel News](https://laravel-news.com/)

- [LaraJobs](https://larajobs.com/)

- [Laravel Forge - Instant PHP Servers](https://forge.laravel.com/)

- [Envoyer - Zero Downtime PHP Deployment](https://envoyer.io/)

- [Laravel Spark](https://spark.laravel.com/)

- [Laravel Nova - Beautifully-designed administration panel for Laravel](https://nova.laravel.com/)

- [Test-Driven Laravel – Learn to build robust, well-designed Laravel applications with TDD.](https://course.testdrivenlaravel.com/)

- [Servers for Hackers](https://serversforhackers.com/)

- [O'Reilly Media - Tech Books and Videos](http://shop.oreilly.com/)

## [Initial Setup Requirements](https://laracasts.com/series/laravel-from-scratch-2018/episodes/2)

> Like any modern PHP framework, 
you'll need to install a few prerequisites to prepare for Laravel. 
Don't worry: this is a one-time job. 
Stick with me, and we'll get through it quickly. 
We'll first install Composer, make it available system-wide, 
and then pull in the Laravel installer. 
This small tool will allow us to run a simple command (laravel new app) 
to instantly generate a fresh Laravel project.

## [Basic Routing](https://laracasts.com/series/laravel-from-scratch-2018/episodes/3)

> When learning a new framework, 
one of your first tasks is to determine how routing is handled. 
Or in other words, when I visit a particular URL in the browser, 
how does my framework route that URL to the necessary logic? 
Let's review the basics in this episode.

## [Blade Layout Files](https://laracasts.com/series/laravel-from-scratch-2018/episodes/4)

> When constructing your views, you're not limited to basic PHP. 
Instead, you can use Blade: Laravel's powerful templating engine. 
We'll talk about Blade more in the future, but for now, 
let's leverage it to create a layout file to reduce duplication and complexity.

```php
@yield('title', 'Laracasts')

@section('title', 'Contact Us')
```

## [Sending Data to Your Views](https://laracasts.com/series/laravel-from-scratch-2018/episodes/5?autoplay=true)

> You'll often need to pass data to your views. 
Perhaps it's a collection from the database, 
or maybe a flash message to confirm a particular user action. 
Let's review how easy this is to do.

```php
<?php
view('welcome', ['foo' => 'bar']);
view('welcome')->with(['foo' => 'bar']);
view('welcome')->withFoo('bar');
```

```php
<?= $foo; ?>
{{ $foo }}
{!! $foo !!}
```
