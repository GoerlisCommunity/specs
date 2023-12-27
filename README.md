# Goerlis Protocol Specifications

The community-driven inscription protocol.

## Genesis

* For faster indexer building, [`gors` snapshot](genesis/gors.json) is provided
* Genesis data is verifiable on [dune](https://dune.com/goerlis/goerlis)

## Basic rules

* Currently, contract interaction is not supported.
* All txs should be sent to the tx sender with 0 value.
* Calldata should be in compact form like `data:,{"p":"grc-20","op":"mint","tick":"gors","amt":"10"}` without `\n` and `space`.
* Parmas should follow the order defined in specs.
* If tx param contains invalid data, the whole tx will be ignored.
* Now the protocol only supports data starting with `data:${mimetype},${data}`
* Empty mime type will be recoginzed as `application/json`

## Global params

* Goerli
  * Confirmation: `6`
* Ethereum mainnet
  * Confirmation: `6`

## Formal Specs

* [`Bridge`](ops/bridge.md)

## Draft Specs

* [`Deploy`](ops/deploy.md)
* [`Mint`](ops/mint.md)
* [`Transfer`](ops/transfer.md)

## TODO Specs

## Pull Requests are welcomed!

## License

CC0 1.0
