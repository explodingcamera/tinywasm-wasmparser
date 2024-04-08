# `tinywasm-wasmparser`

[![docs.rs](https://img.shields.io/docsrs/tinywasm-wasmparser?logo=rust)](https://docs.rs/tinywasm-wasmparser) [![Crates.io](https://img.shields.io/crates/v/tinywasm-wasmparser.svg?logo=rust)](https://crates.io/crates/tinywasm-wasmparser) [![Crates.io](https://img.shields.io/crates/l/tinywasm-wasmparser.svg)](./LICENSE-APACHE)

No_std compatible fork of the [wasmparser (200.0.0)](https://github.com/bytecodealliance/wasm-tools) crate for internal use in the [tinywasm](https://crates.io/crates/tinywasm) project.
Since there doesn't seem to be interest in making the original crate no_std compatible (see [issue](https://github.com/bytecodealliance/wasm-tools/pull/364)), this fork was created. There's also another [no_std fork](https://crates.io/crates/wasmparser_nostd) of the original crate, but it's not actively maintained.

This crate can have breaking changes at any time for the sake of the tinywasm project, so it's not recommended to use it directly.

## Changes from the original crate

- Added `no_std` support
- Added default implementation for all `visit_*` methods in the `VisitOperator` trait

# License

This project is licensed under the Apache 2.0 license with the LLVM exception. See LICENSE for more details.
