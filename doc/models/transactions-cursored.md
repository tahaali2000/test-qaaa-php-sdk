
# Transactions Cursored

## Structure

`TransactionsCursored`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `data` | [`?(Transaction[])`](../../doc/models/transaction.md) | Optional | - | getData(): ?array | setData(?array data): void |
| `nextCursor` | `?string` | Optional | Cursor for the next page of results. | getNextCursor(): ?string | setNextCursor(?string nextCursor): void |

## Example (as JSON)

```json
{
  "nextCursor": "txn_abc999",
  "data": [
    {
      "id": "id0",
      "amount": 43.32,
      "timestamp": "2016-03-13T12:52:32.123Z"
    },
    {
      "id": "id0",
      "amount": 43.32,
      "timestamp": "2016-03-13T12:52:32.123Z"
    }
  ]
}
```

