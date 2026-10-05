<!-- tyhp-readme:start -->
# tyhpdef/illuminate-json-schema

Tyhp type definitions for `illuminate/json-schema` `13.32.0`.

```bash
composer require --dev tyhpdef/illuminate-json-schema:13.32.0
```

This is a metapackage. Composer also installs `tyhpdef/illuminate-json-schema-impl` (type files).
Require **this** name, not `tyhpdef/illuminate-json-schema-impl`.

See https://tyhplang.com.

## Maintain `illuminate/json-schema`? Ship the types yourself

If you are a Packagist maintainer of `illuminate/json-schema`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/illuminate-json-schema-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `illuminate/json-schema` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/illuminate-json-schema": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `illuminate/json-schema` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `illuminate/json-schema` with a real constraint,
   `"replace": { "tyhpdef/illuminate-json-schema": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `illuminate/json-schema` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/illuminate-json-schema` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
