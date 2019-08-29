# Pigeon
[![Build Status](https://travis-ci.org/convenia/Pigeon.svg?branch=develop)](https://travis-ci.org/convenia/Pigeon)
[![StyleCI](https://github.styleci.io/repos/201348189/shield?branch=develop)](https://github.styleci.io/repos/201348189)

Pigeon is a Laravel package for dealing with AMQP messaging messaging with easy syntax on top of php-amqplib.

## Installation

Use the package manager [composer](https://getcomposer.org/) to install

```bash
composer require convenia/pigeon
```

Edit your `.env` file and put he the following environment variables with your environments values
```dotenv
PIGEON_DRIVER=rabbit
PIGEON_ADDRESS=localhost # Your AMQP host
PIGEON_PORT=15672 # Your AMQP port
PIGEON_USER=guest
PIGEON_PASSWORD=guest
PIGEON_VHOST=/
PIGEON_EXCHANGE=application # Your applciaton default exchange
PIGEON_EXCHANGE_TYPE=fanout # Your applciaton default exchange type
PIGEON_CONSUMER_TAG=application # Your applciaton name
```

## Change log
Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[GPL V3](https://choosealicense.com/licenses/gpl-v3/)
