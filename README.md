# 🎩⚡ powerpack

[![Crates.io Version](https://img.shields.io/crates/v/powerpack.svg)](https://crates.io/crates/powerpack)
[![Docs.rs Latest](https://img.shields.io/badge/docs.rs-latest-blue.svg)](https://docs.rs/powerpack)
[![Build Status](https://img.shields.io/github/workflow/status/rossmacarthur/powerpack/build/trunk)](https://github.com/rossmacarthur/powerpack/actions?query=workflow%3Abuild)

Supercharge your [Alfred] workflows by building them in Rust 🦀!

[Alfred]: https://www.alfredapp.com

## 🚀 Getting started

This project contains a `powerpack` crate which provides types for developing
script filter Alfred workflows in Rust. It also provides a command line tool to
initialize, build, and install  workflows built using the `powerpack` crate.

Firstly, install the command line tool.
```sh
cargo install powerpack-cli
```

Now create a new project using a similar API as `cargo new` or `cargo init`.
```sh
powerpack new myworkflow
```

This will create a new Rust project as well as a `workflow/` directory
containing information about your Alfred workflow. The following will create
a release build of the workflow and copy it to the `workflow/` directory.
```sh
powerpack build
```

Now you can link it. The following will symlink the `workflow/` directory to
the Alfred preferences folder.
```sh
powerpack link
```

To package a `.alfredworkflow` file for release you can run the following.
```sh
powerpack package
```

## 💡 Examples

The following projects are built using `powerpack`.

- [emojis.alfred-workflow](https://github.com/rossmacarthur/emojis.alfred-workflow)

## License

Licensed under either of

- Apache License, Version 2.0 ([LICENSE-APACHE](LICENSE-APACHE) or
  http://www.apache.org/licenses/LICENSE-2.0)
- MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.
