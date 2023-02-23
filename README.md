# toml++

[![build2](https://github.com/build2-packaging/tomlplusplus/actions/workflows/build2.yml/badge.svg)](https://github.com/build2-packaging/tomlplusplus/actions/workflows/build2.yml)

This project builds and defines the build2 package for the [toml++](https://marzer.github.io/tomlplusplus/) library.

The packaging code is licensed under the MIT License, the upstream artifacts are licensed under the terms and conditions of toml++.

## Usage

You can simply add this package as dependency to your project by specifying it in your `manifest`:

```
depends: libtoml++ ^1.0.0
```

Then import your required targets

```
import libs = libtoml++%lib{toml++}
```

This library offers a big range of options (though the default values are reasonable), so have a look at the official [upstream code](https://github.com/nanomsg/nng) and the [root.build](libnng/build/root.build).

## Issues

* no TLS support: wolfssl and/or mbedtls need to be available as packages first
