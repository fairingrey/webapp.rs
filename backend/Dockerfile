FROM rustlang/rust:nightly

RUN rustup component add \
    clippy-preview \
    rls-preview \
    rust-analysis \
    rustfmt-preview

RUN cargo install cargo-watch

RUN cargo install diesel_cli --no-default-features --features postgres

WORKDIR /usr/src

EXPOSE 30080 30081 30082