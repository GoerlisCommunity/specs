# Goerlis Protocol Specifications

The community-driven inscription protocol.

## Genesis

* For faster indexer building, [`gors` snapshot](genesis/gors.json) is provided
* Genesis data is verifiable on [dune](https://dune.com/goerlis/goerlis)

## Basic rules

* Currently, contract interaction is not supported.
* All txs should be sent to the tx sender with 0 value.
* Now the protocol only supports data starting with `data:,`

## Draft Specs

* [`Deploy`](ops/deploy.md)
* [`Mint`](ops/mint.md)
* [`Bridge`](ops/bridge.md)

## TODO Specs

* `Transfer` - there's no transfer spec being proposed yet

## Pull Requests are welcomed!

## License

CC0 1.0
