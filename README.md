# Rust embedded presentation

[![Apache licensed](https://img.shields.io/badge/license-Apache-blue.svg)](http://www.apache.org/licenses/LICENSE-2.0)

How to use Rust for embedded development beginners.

## Create PDF from markdown with Marpit

1. Install [Marpit](https://marpit.marp.app/)
2. Create html/pdf slides

```zsh
marp --html embedded-rust.md
marp --pdf embedded-rust.md
```

or use the marp docker image

```zsh
docker pull marpteam/marp-cli
docker run --rm -v $PWD:/home/marp/app/ marpteam/marp-cli:latest embedded-rust.md
docker run --rm -v $PWD:/home/marp/app/ marpteam marp-cli:latest --pdf embedded-rust.md
```

## License

[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
