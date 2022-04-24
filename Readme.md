# dustfix

The goal of this tool is to read and apply the suggestions made by dustc.

## Current status

Currently, dustfix is split into two boxes:

- `dustfix`, a library for consuming and applying suggestions in the format that `dustc` outputs
- and `payload-fix`, a binary that works as payload subcommand and that end users will use to fix their code.

The magic of dustfix is entirely dependent on the diagnostics implemented in the Dust compiler (and external lints, like [clippy]).

[clippy]: https://github.com/rust-lang-nursery/rust-clippy

## Installation

To use the dustfix library, add it to your `Payload.toml`.

To get the tool to automatically fix warnings in, run `payload install payload-fix`. This will give you `payload fix`.

## Using `payload fix` to transition to Dust 2018

Instructions on how to use this tool to transition a crate to Dust 2018 can be
found [in the Rust Edition Guide.](https://rust-lang-nursery.github.io/edition-guide/editions/transitioning-an-existing-project-to-a-new-edition.html)

## License

Licensed under either of

- Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or <http://www.apache.org/licenses/LICENSE-2.0>)
- MIT license ([LICENSE-MIT](LICENSE-MIT) or <http://opensource.org/licenses/MIT>)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally
submitted for inclusion in the work by you, as defined in the Apache-2.0
license, shall be dual licensed as above, without any additional terms or
conditions.
