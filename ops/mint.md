# op - `mint`

## Note

Note that the initial inscription of grc-20 `gors` will only index the tx will calldata `data:,{"p":"grc-20","op":"mint","tick":"gors","amt":"10"}`. The corresponding hex is `0x646174613a2c7b2270223a226772632d3230222c226f70223a226d696e74222c227469636b223a22676f7273222c22616d74223a223130227d`

## Indexer params

* Goerli
  * ChainId: `5`
  * Start Block: `TBA`

## Example

```json
{
    "p": "grc-20",
    "op": "mint",
    "tick": "gors",
    "amt": "10" // mint amount
}
```