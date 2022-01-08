# PHP DotEnv Loader

[![Latest Stable Version](http://poser.pugx.org/murilo-perosa/dot-env/v)](https://packagist.org/packages/murilo-perosa/dot-env) 
[![Total Downloads](http://poser.pugx.org/murilo-perosa/dot-env/downloads)](https://packagist.org/packages/murilo-perosa/dot-env) 
[![License](http://poser.pugx.org/murilo-perosa/dot-env/license)](https://packagist.org/packages/murilo-perosa/dot-env) 
[![PHP Version Require](http://poser.pugx.org/murilo-perosa/dot-env/require/php)](https://packagist.org/packages/murilo-perosa/dot-env)

Simple library to load and get values from `.env` file(s).

## Install

```bash
composer require murilo-perosa/dot-env
```

## How to Use

### Namespace

```php
use MuriloPerosa\DotEnv\DotEnv;
```

### Load File
```php
// enter path to .env file
(new DotEnv(__DIR__ . '/../.env'))->load();
```

### Get Values
```php

// php implementation
$value = getenv('YOUR_KEY');

// package implementation
$value = DotEnv::get('YOUR_KEY');

// package implementation with default value
$value = DotEnv::get('YOUR_KEY', 'DEFAULT_VALUE');
```
