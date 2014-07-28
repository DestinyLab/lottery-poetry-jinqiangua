# Lottery-Poetry-JinQianGua（金錢卦）

Lottery-Poetry-JinQianGua is the data of Lottery-Poetry-Engine.

## Requirement

 - PHP >=5.4

## Installing via Composer

The recommended way to install Lottery-Poetry-JinQianGua is through Composer.

```bash
# Install Composer
curl -sS https://getcomposer.org/installer | php
```

Next, update your project's composer.json file to include Lottery-Poetry-JinQianGua:

```json
{
    "require": {
        "destinylab/lottery-poetry-jinqiangua": "dev-master"
    }
}
```

## Usage

```php
<?php

require_once 'vendor/autoload.php';

$suit = new DestinyLab\LotteryPoetry\JinQianGua([__DIR__.'/resources'], 'yml');
$engine = new DestinyLab\LotteryPoetry\Engine($suit);

// get contents
$engine->draw();

// get only key
$engine->draw(true);
```

## License

MIT