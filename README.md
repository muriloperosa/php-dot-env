# PHP DotEnv Loader

Simple library to load and get values from `.env` file(s).

## Install

```bash
...
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
