# Transaction

```php
$transactionController = $client->getTransactionController();
```

## Class Name

`TransactionController`

## Methods

* [Fetch With Cursor](../../doc/controllers/transaction.md#fetch-with-cursor)
* [Fetch With Link](../../doc/controllers/transaction.md#fetch-with-link)
* [Fetch With Offset](../../doc/controllers/transaction.md#fetch-with-offset)


# Fetch With Cursor

Fetch transactions using Cursor-based Pagination

```php
function fetchWithCursor(?string $cursor = null, ?int $limit = 10): TransactionsCursored
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `cursor` | `?string` | Query, Optional | The unique identifier (cursor) to fetch the next set of results. |
| `limit` | `?int` | Query, Optional | Number of transactions per page.<br><br>**Default**: `10`<br><br>**Constraints**: `>= 1`, `<= 100` |

## Response Type

[`TransactionsCursored`](../../doc/models/transactions-cursored.md)

## Example Usage

```php
$cursor = 'txn_abc123';

$limit = 10;

$result = $transactionController->fetchWithCursor(
    $cursor,
    $limit
);
```


# Fetch With Link

Fetch transactions using Link-based Pagination

```php
function fetchWithLink(?int $page = 1, ?int $size = 10): TransactionsLinked
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `page` | `?int` | Query, Optional | The page number to fetch.<br><br>**Default**: `1`<br><br>**Constraints**: `>= 1` |
| `size` | `?int` | Query, Optional | Number of transactions per page.<br><br>**Default**: `10`<br><br>**Constraints**: `>= 1`, `<= 100` |

## Response Type

[`TransactionsLinked`](../../doc/models/transactions-linked.md)

## Example Usage

```php
$page = 1;

$size = 10;

$result = $transactionController->fetchWithLink(
    $page,
    $size
);
```


# Fetch With Offset

Fetch transactions using Offset-based Pagination

```php
function fetchWithOffset(?int $offset = 0, ?int $limit = 10): TransactionsOffset
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `offset` | `?int` | Query, Optional | The number of records to skip before selecting transactions.<br><br>**Default**: `0`<br><br>**Constraints**: `>= 0` |
| `limit` | `?int` | Query, Optional | Number of transactions per page.<br><br>**Default**: `10`<br><br>**Constraints**: `>= 1`, `<= 100` |

## Response Type

[`TransactionsOffset`](../../doc/models/transactions-offset.md)

## Example Usage

```php
$offset = 0;

$limit = 10;

$result = $transactionController->fetchWithOffset(
    $offset,
    $limit
);
```

