<p align="center">
  <img src="https://raw.githubusercontent.com/php-plus/engine/master/art/logo.gif" width="334" alt="PHP Insights">
  <img src="https://raw.githubusercontent.com/php-plus/engine/master/art/preview.png" width="882" alt="PHP Insights Preview">
  <p align="center">
    <a href="https://travis-ci.org/php-plus/engine"><img src="https://img.shields.io/travis/php-plus/engine/master.svg" alt="Build Status"></a>
    <a href="https://packagist.org/packages/php-plus/engine"><img src="https://poser.pugx.org/php-plus/engine/d/total.svg" alt="Total Downloads"></a>
    <a href="https://packagist.org/packages/php-plus/engine"><img src="https://poser.pugx.org/php-plus/engine/v/stable.svg" alt="Latest Version"></a>
    <a href="https://packagist.org/packages/php-plus/engine"><img src="https://poser.pugx.org/php-plus/engine/license.svg" alt="License"></a>
  </p>
  <p align="center">
    <strong>For full documentation, visit <a href="https://php-plus.com">php-plus.com</a></strong>.
  </p>
</p>

**Plus** is superset of PHP that makes PHP cool again. It was created by
**[Nuno Maduro](https://github.com/nunomaduro)**, and it's built on top of
**[Pre](https://preprocess.io)** - a preprocessing tool for PHP. **Plus**'s art work
is provided by **[Caneco](https://twitter.com/caneco)**.

Plus is a **runtime compiler** that adds features to PHP - It's also a package that you can require using
composer, and is mainly used to add features and syntactic sugar to existant PHP code. Of course, those features
arrive in PHP using runtime source code transformations.

Enjoy a simple and powerful syntax that enables developers to build very complex applications far more quickly
than before. Short closures, types, enumerations are just a few examples of what you get using **Plus**.

## 🚀 Try Plus in 10 seconds

> Note: Plus is still work in progress and it's not out yet.

- First, install:
```
composer require php-plus/engine
```

- Then, in your editor, add the following declare:
```php
<?php

declare(plus=1);

class User {
    // A readonly property cannot be assigned after the constructor exits
    public readonly string $name;

    // No need for the `t_function` keyword
    public __construct(string $name) {
        $this->name = $name;
    }

    // One expression functions with return statement
    public getUppercasedName(): string => strtoupper($this->name)
}
```

## 💖 Support the development
**Do you like this project? Support it by donating**

- PayPal: [Donate](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=66BYDWAT92N6L)
- Patreon: [Donate](https://www.patreon.com/nunomaduro)

**Plus** is open-sourced software licensed under the [MIT license](LICENSE.md).
