# ZelloWork API Wrapper

This provides a Laravel style wrapper for ZelloWork API.

For more information see [https://github.com/zelloptt/zellowork-server-api-libs](https://github.com/zelloptt/zellowork-server-api-libs)

## Install

Require this package with composer using the following command:

```bash
$ composer require mobiadroit/zello-work-api
```

### Configuration

See [Authentication](#Authentication) section on how to use these environment variables.

| Variable name                | Default                           | Description                                   |
| ---------------------------- | --------------------------------- | --------------------------------------------- |
| `ZELLO_USER`                 |                                   | Your Zello User to use with API               |
| `ZELLO_PASSWORD`             |                                   | Your Zello User password                      |
| `ZELLO_API_KEY`              |                                   | Your Zello API key                            |
| `ZELLO_HOST`                 |                                   | Your ZelloWork Host                           |

## Authentication

Authentication is done via the Zello user and password as well as the API Key value. Ensure you do not commit your Zello user and password information to any repositories and use ENV variables

#### Create a Key

Go to the ***Administration -> API Keys*** in your ZelloWork Console.

Click **Create Token**.

Remember to download the key file you get at the end! This is the only time it is shown.

#### Configuration

Add the following lines to the .env file:

```sh
ZELLO_USER="USER"
ZELLO_PASSWORD="PASSWORD"
ZELLO_API_KEY="API KEY"
ZELLO_HOST="{network}.zellowork.com"
```
Replace {network} with your ZelloWork Network Name

## License

The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
