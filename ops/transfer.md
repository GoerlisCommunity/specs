# op - `transfer`

Adopted from [ierc-20](https://docs.ierc20.com/devs/ierc-20/transfer)

## TODO

Smart Contract Transfer Spec.

## Indexer params

* Ethereum Mainnet
  * ChainId: `1`
  * Start Block: `18898123`

## Example

```json
{
  "p": "grc-20",
  "op": "transfer", //transfer operation
  "tick": "gors",
  "to": [ //batch transfer, the sum of amt must equal the previous amt param
    {
      "recv": "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48", //receiver checksummed address
      "amt": "50" //receiver amount
    },
    {
      "recv": "0x0000000000085d4780B73119b644AE5ecd22b376",
      "amt": "50"
    }
  ]
}
```