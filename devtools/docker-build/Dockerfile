FROM ubuntu:18.04
LABEL maintainer="yejiayu.fe@gmail.com"

COPY target/release/huobi-chain .
COPY config/config.toml devtools/config/config.toml
COPY config/genesis.toml devtools/config/genesis.toml

EXPOSE 1337 8000
CMD ["./huobi-chain", "-c", "devtools/config/config.toml", "-g", "devtools/config/genesis.toml"]
