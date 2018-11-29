FROM rustlang/rust:nightly

RUN rustup component add \
    clippy-preview \
    rls-preview \
    rust-analysis \
    rustfmt-preview

RUN rustup target add \
    --toolchain nightly \
    wasm32-unknown-unknown

RUN cargo install cargo-web

WORKDIR /usr/src

EXPOSE 8000
