
# Links

## Structure

`Links`

## Fields

| Name | Type | Tags | Description | Getter | Setter |
|  --- | --- | --- | --- | --- | --- |
| `first` | `?string` | Optional | - | getFirst(): ?string | setFirst(?string first): void |
| `last` | `?string` | Optional | - | getLast(): ?string | setLast(?string last): void |
| `prev` | `?string` | Optional | - | getPrev(): ?string | setPrev(?string prev): void |
| `next` | `?string` | Optional | - | getNext(): ?string | setNext(?string next): void |

## Example (as JSON)

```json
{
  "first": "/transactions/links?page=1&size=10",
  "last": "/transactions/links?page=5&size=10",
  "prev": "/transactions/links?page=1&size=10",
  "next": "/transactions/links?page=3&size=10"
}
```

