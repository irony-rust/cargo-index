Rust crate index
======================

This is the crate index for the alternative crate registry instance running locally.

This repository follows the rules and layout specified in the [Cargo's Alternative Registries RFC].  
It is maintained and kept up-to-date automatically.

This index (and, by extension, the registry) allows crates to only depend on other crates stored in either this registry or [crates.io].

How to use this index
---------------------

If you want to use this index, you can follow these steps:

- Edit or create the `~/.cargo/config` file, and add the following code:
```toml
[registries.irony-rust]
index = "https://github.com/irony-rust/cargo-index"
```
- Then, run `cargo login --registry alexandrie` and enter your author token.
- You can now use the registry using `cargo publish --registry alexandrie` or `cargo search --registry alexandrie`

[Crates]: https://github.com/irony-rust/cargo-index
[crates.io]: https://crates.io
[Cargo's Alternative Registries RFC]: https://github.com/rust-lang/rfcs/blob/master/text/2141-alternative-registries.md#registry-index-format-specification
