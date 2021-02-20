# Node runtime types for `pro!`

Defines types for [pro!](https://github.com/tetcoin/pro) smart contracts targeting [Substrate's `node-runtime`](https://github.com/paritytech/substrate/blob/master/bin/node/runtime/src/lib.rs).

Supplies an implementation of the [pro! `EnvTypes` trait](https://github.com/tetcoin/pro/blob/master/core/src/env/types.rs#L128).

See `pro!` [examples](./examples) for usage.

## Requirements
```
rustup component add rust-src --toolchain nightly
rustup target add wasm32-unknown-unknown --toolchain nightly
rustup target add wasm32-unknown-unknown --toolchain stable
cargo install cargo-contract --vers 0.6.1 --force
```

## Build

### Runtime Dependencies
```
cargo +nightly build --release
```

### pro! Smart Contract
```
cargo +nightly contract build
cargo +nightly contract generate-metadata
```

## Test
```
cargo +nightly test
```
