# rust-llvm-wasi

LLVM and LLD, patched so they can be built to run on a WASI host
(`wasm32-wasip1-threads`), for building a WebAssembly-hosted `rustc`. It is the
LLVM submodule of [rad-rs/rust-wasi](https://github.com/rad-rs/rust-wasi); see
[rad-rs/wasm-rustc-windows](https://github.com/rad-rs/wasm-rustc-windows) for
how the pieces fit together.

**This is not a general-purpose LLVM.** For ordinary use, build
[llvm/llvm-project](https://github.com/llvm/llvm-project) or Rust's own fork,
[rust-lang/llvm-project](https://github.com/rust-lang/llvm-project).

## Credits

- **Catherine and the YoWASP project**, who wrote the WASI patch this is based
  on; their commit is the first one on `wasi-host/23.1`, with her authorship
  preserved. YoWASP now lives on Codeberg:
  <https://codeberg.org/YoWASP/llvm-project>.
- **The Rust project**, for the LLVM fork this builds on, and **the LLVM
  project**.

## Licence

As LLVM: Apache License v2.0 with LLVM Exceptions. See `LICENSE.TXT` on the
patch branch.
