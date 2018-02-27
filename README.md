# `robots.txt` and `robots` meta parser

[![Latest Version on Packagist](https://img.shields.io/packagist/v/spatie/robots-txt.svg?style=flat-square)](https://packagist.org/packages/spatie/robots-txt)
[![Build Status](https://img.shields.io/travis/spatie/robots-txt/master.svg?style=flat-square)](https://travis-ci.org/spatie/robots-txt)
[![SensioLabsInsight](https://img.shields.io/sensiolabs/i/xxxxxxxxx.svg?style=flat-square)](https://insight.sensiolabs.com/projects/xxxxxxxxx)
[![Quality Score](https://img.shields.io/scrutinizer/g/spatie/robots-txt.svg?style=flat-square)](https://scrutinizer-ci.com/g/spatie/robots-txt)
[![Total Downloads](https://img.shields.io/packagist/dt/spatie/robots-txt.svg?style=flat-square)](https://packagist.org/packages/spatie/robots-txt)

Determine if a page may be crawled from robots.txt and robots meta tags.

## Installation

You can install the package via composer:

```bash
composer require spatie/robots-txt
```

## Usage

``` php
$robots = Robots::create(__DIR__ . '/data/robots.txt');

$robots->isAllowed('/admin');

$robots->mayFollow('/page-with-no-follow');
```

You can also specify a user agent:

``` php
$robots = Robots::create(__DIR__ . '/data/robots.txt', 'UserAgent007');
```

### Testing

``` bash
composer test
```

### Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

### Security

If you discover any security related issues, please email freek@spatie.be instead of using the issue tracker.

## Postcardware

You're free to use this package, but if it makes it to your production environment we highly appreciate you sending us a postcard from your hometown, mentioning which of our package(s) you are using.

Our address is: Spatie, Samberstraat 69D, 2060 Antwerp, Belgium.

We publish all received postcards [on our company website](https://spatie.be/en/opensource/postcards).

## Credits

- [Brent Roose](https://github.com/brendt_gd)
- [All Contributors](../../contributors)

## Support us

Spatie is a webdesign agency based in Antwerp, Belgium. You'll find an overview of all our open source projects [on our website](https://spatie.be/opensource).

Does your business depend on our contributions? Reach out and support us on [Patreon](https://www.patreon.com/spatie). 
All pledges will be dedicated to allocating workforce on maintenance and new awesome stuff.

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.