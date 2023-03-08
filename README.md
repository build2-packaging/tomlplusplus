# toml++

[![build2](https://github.com/build2-packaging/tomlplusplus/actions/workflows/build2.yml/badge.svg)](https://github.com/build2-packaging/tomlplusplus/actions/workflows/build2.yml)

This project builds and defines the build2 package for the [toml++](https://marzer.github.io/tomlplusplus/) library.

The packaging code is licensed under the MIT License, the upstream artifacts are licensed under the terms and conditions of toml++.

## Usage

You can simply add this package as dependency to your project by specifying it in your `manifest`:

```
depends: libtomlplusplus ^3.3.0
```

Then import your required targets

```
import libs = libtomlplusplus++%lib{tomlplusplus++}
```

By the default the library is compiled and uses exceptions. You cange this behaviour by specifying the configs explicilty:

```
config.libtomlplusplus.use_header_only = true
config.libtomlplusplus.use_exceptions = false
```

