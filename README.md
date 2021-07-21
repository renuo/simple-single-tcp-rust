# Simple TCP server

Run it with

```sh
./simple-single-tcp
```

Cross-compile for Heroku with:

```sh
CARGO_TARGET_X86_64_UNKNOWN_LINUX_GNU_LINKER=x86_64-unknown-linux-gnu-gcc \
cargo build --target=x86_64-unknown-linux-gnu --release
```

If you're on MacOS, you'll need a linker first:

```sh
rustup target add x86_64-unknown-linux-gnu

# Install a pre-built cross compiler
brew tap SergioBenitez/osxct
brew install x86_64-unknown-linux-gnu
```
