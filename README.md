<!-- tyhp-readme:start -->
# tyhpdef/php-amqplib-php-amqplib

Tyhp type definitions for `php-amqplib/php-amqplib` `3.7.4`.

```bash
composer require --dev tyhpdef/php-amqplib-php-amqplib:3.7.4
```

This is a metapackage. Composer also installs `tyhpdef/php-amqplib-php-amqplib-impl` (type files).
Require **this** name, not `tyhpdef/php-amqplib-php-amqplib-impl`.

See https://tyhplang.com.

## Maintain `php-amqplib/php-amqplib`? Ship the types yourself

If you are a Packagist maintainer of `php-amqplib/php-amqplib`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/php-amqplib-php-amqplib-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `php-amqplib/php-amqplib` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/php-amqplib-php-amqplib": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `php-amqplib/php-amqplib` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `php-amqplib/php-amqplib` with a real constraint,
   `"replace": { "tyhpdef/php-amqplib-php-amqplib": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `php-amqplib/php-amqplib` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/php-amqplib-php-amqplib` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
