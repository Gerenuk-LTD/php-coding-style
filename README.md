# Gerenuk's Coding Style

## PHP (Laravel Pint)

### Installation

1\. Add the repository to your `composer.json` using either the JSON format:

```json
"repositories": {
    "gerenuk/php-coding-style": {
        "type": "vcs",
        "url": "https://github.com/Gerenuk-LTD/php-coding-style.git"
    }
},
```

Or the CLI command:

```sh
composer config repositories.gerenuk/php-coding-style '{"type": "vcs", "url": "https://github.com/Gerenuk-LTD/php-coding-style.git"}' --file composer.json
```

2\. Include `gerenuk/php-coding-style` in your project's dev dependencies:

```sh
composer require --dev gerenuk/php-coding-style
```

### Usage

Run the Pint command to apply the Gerenuk coding style:

```sh
./vendor/bin/pint --config vendor/gerenuk/php-coding-style/pint.json
```

You can also add a script to your `composer.json` for quicker style application:

```sh
composer config scripts.pint 'pint --config vendor/gerenuk/php-coding-style/pint.json' --file composer.json
```

Apply Gerenuk's coding style using the script:

```sh
composer pint
```
