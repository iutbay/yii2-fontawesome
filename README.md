Font Awesome helper for Yii2
============================

[Font Awesome](http://fortawesome.github.io/Font-Awesome/) helper for Yii2.

Installation
------------
The preferred way to install this helper is through [composer](http://getcomposer.org/download/).

Either run

```
php composer.phar require "iutbay/yii2-fontawesome" "*"
```

or add

```json
"iutbay/yii2-fontawesome" : "*"
```

to the require section of your application's `composer.json` file.

Assets
------
To include Font Awesome assets, you should register it in view :

```php
\iutbay\yii2-fontawesome\FontAwesomeAsset::register($this);
```

Or as dependency in your app asset bundle :

```php
public $depends = [
    'iutbay\yii2fontawesome\FontAwesomeAsset',
];
```

Usage
-----

```php
use iutbay\yii2fontawesome\FontAwesome as FA;

// home icon : <i class="fa fa-home"></i>
echo FA::icon('home');

// 2x home icon : <i class="fa fa-home fa-2x"></i>
echo FA::icon('home 2x');

// fixed width home icon : <i class="fa fa-home fa-fw"></i>
echo FA::icon('home fw');
```
