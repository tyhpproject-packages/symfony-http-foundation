<!-- tyhp-readme:start -->
# tyhpdef/symfony-http-foundation

Tyhp type definitions for `symfony/http-foundation` `8.1.7`.

```bash
composer require --dev tyhpdef/symfony-http-foundation:8.1.7
```

This is a metapackage. Composer also installs `tyhpdef/symfony-http-foundation-impl` (type files).
Require **this** name, not `tyhpdef/symfony-http-foundation-impl`.

See https://tyhplang.com.

## Maintain `symfony/http-foundation`? Ship the types yourself

If you are a Packagist maintainer of `symfony/http-foundation`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-http-foundation-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/http-foundation` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-http-foundation": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/http-foundation` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/http-foundation` with a real constraint,
   `"replace": { "tyhpdef/symfony-http-foundation": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/http-foundation` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-http-foundation` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
