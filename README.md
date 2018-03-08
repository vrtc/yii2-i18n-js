# yii2-i18n-js

- [Installation](#installation)
- [Usage](#usage)

## Installation

``` shell
composer require w3lifer/yii2-i18n-js
```

1. Add this to your application configuration:

``` php
<?php

return [
    // ...
    'components' => [
        // ...
        'i18nJs' => [
            'class' => 'w3lifer\yii2\I18nJs',
        ],
        // ...
    ],
    // ...
];
```

2. Initialize the component anywhere, for example in the configuration:

``` php
<?php

return [
    // ...
    'components' => [
        // ...
        'i18nJs' => [
            'class' => 'w3lifer\yii2\I18nJs',
        ],
        // ...
    ],
    // ...
    'on afterRequest' => function () {
        Yii::$app->i18nJs;
    },
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
