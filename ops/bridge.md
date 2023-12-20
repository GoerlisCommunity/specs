# op - `bridge-send`, `bridge-recv`

## Indexer params

After `confirmation` blocks, `bridge-send` tx will be confrimed by indexer and can be claimed on dst chain.

Only `bridge-recv` txs after the confirmation timestamp on src chain will be processed by indexer.

### Supported source chain

* Goerli
  * ChainId: `5`
  * Start Block: `TBA`

### Supported destination chain

* Ethereum Mainnet
  * ChainId: `1`
  * Start Block: `TBA`

## Example

```json
{
    "p": "grc-20",
    "op": "bridge-send",
    "tick": "gors",
    "dst": "1", // destination chainid
    "amt": "1000" // bridge amount
}

{
    "p": "grc-20",
    "op": "bridge-recv",
    "tick": "gors",
    "src": "5",
    "hash": "0x0000000000000000000000000000000000000000000000000000000000000000" // use the `bridge-send` hash on the source chain
}
```