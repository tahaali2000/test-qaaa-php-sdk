
# Transactions Linked

## Structure

`TransactionsLinked`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `data` | [`?(Transaction[])`](../../doc/models/transaction.md) | Optional | - | getData(): ?array | setData(?array data): void |
| `links` | [`?Links`](../../doc/models/links.md) | Optional | - | getLinks(): ?Links | setLinks(?Links links): void |

## Example (as JSON)

```json
{
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
    },
    {
      "id": "id0",
      "amount": 43.32,
      "timestamp": "2016-03-13T12:52:32.123Z"
    }
  ],
  "links": {
    "first": "first0",
    "last": "last4",
    "prev": "prev8",
    "next": "next2"
  }
}
```

