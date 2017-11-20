This is a Laravel 5 package that provides h_n_s management facility for lavalite framework.

## Installation

Begin by installing this package through Composer. Edit your project's `composer.json` file to require `dexit/h_n_s`.

    "dexit/h_n_s": "dev-master"

Next, update Composer from the Terminal:

    composer update

Once this operation completes execute below cammnds in command line to finalize installation.

```php
Dexit\HNS\Providers\HNSServiceProvider::class,

```

And also add it to alias

```php
'HNS'  => Dexit\HNS\Facades\HNS::class,
```

Use the below commands for publishing

Migration and seeds

    php artisan vendor:publish --provider="Dexit\HNS\Providers\HNSServiceProvider" --tag="migrations"
    php artisan vendor:publish --provider="Dexit\HNS\Providers\HNSServiceProvider" --tag="seeds"

Configuration

    php artisan vendor:publish --provider="Dexit\HNS\Providers\HNSServiceProvider" --tag="config"

Language

    php artisan vendor:publish --provider="Dexit\HNS\Providers\HNSServiceProvider" --tag="lang"

Views public and admin

    php artisan vendor:publish --provider="Dexit\HNS\Providers\HNSServiceProvider" --tag="view-public"
    php artisan vendor:publish --provider="Dexit\HNS\Providers\HNSServiceProvider" --tag="view-admin"

Publish admin views only if it is necessary.

## Usage


