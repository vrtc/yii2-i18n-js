# yii2-i18n-js

- [Installation](#installation)
- [Usage](#usage)

## Installation

``` shell
composer require w3lifer/yii2-i18n-js
```

Add this to your application configuration:

``` php
<?php

return [
    // ...
    'bootstrap' => [
        // ...
        'i18nJs' => [
            'class' => 'w3lifer\yii2\I18nJs',
        ],
        // ...
    ],
    // ...
];
```

## Usage

``` js
$(function () {
  console.log(yii.t('app', 'Hello'));
  console.log(yii.t('app', 'Hello, World!'));
  console.log(yii.t('app', 'Hello, {username}!', {username: 'John'}));
  console.log(yii.t('app', 'Hello, {0}!', ['John']));
  console.log(yii.t('app', 'Hello, {0} {1}!', ['John', 'Doe']));
});
```
