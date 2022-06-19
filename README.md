# WP-Encrypt

Encrypts and decrypts data using the WordPress Salts and OpenSSL


## Installation

Use the package manager [composer](https://getcomposer.org/) to install WP-Encrypt.

```bash
composer require khorshid/wp-encrypt
```

## Usage

```php
use WP_Encryption\Encryption;

...

$encrypted_data = (new Encryption)->encrypt( $data );
// $encrypted_data is encrypted and safe to store in database.

$decrypted_data = (new Encryption)->decrypt( $encrypted_data );
// $encrypted_data = $data

```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[GPL3](https://www.gnu.org/licenses/gpl-3.0.en.html)
