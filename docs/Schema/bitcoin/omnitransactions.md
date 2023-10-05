---
title: Bitcoin OmniTransactions API
---

<head>
<meta name="title" content="Bitcoin OmniTransactions API"/>
<meta name="description" content="Retrieve Bitcoin Omni Transactions with advanced filtering options and access details on transactions, fees, and more from the Bitcoin network."/>

<meta name="keywords" content="Bitcoin api, Bitcoin python api, Bitcoin nft api, Bitcoin scan api, Bitcoin matic api, Bitcoin api docs, Bitcoin crypto api, Bitcoin blockchain api,matic network api"/>
<meta name="robots" content="index, follow"/>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
<meta name="language" content="English"/>

<!-- Open Graph / Facebook -->
<meta property="og:type" content="website" />
<meta property="og:title" content="Bitcoin OmniTransactions API" />
<meta property="og:description" content="Retrieve Bitcoin Omni Transactions with advanced filtering options and access details on transactions, fees, and more from the Bitcoin network." />

<!-- Twitter -->
<meta property="twitter:card" content="summary_large_image" />
<meta property="twitter:title" content="Bitcoin OmniTransactions API" />
<meta property="twitter:description" content="Retrieve Bitcoin Omni Transactions with advanced filtering options and access details on transactions, fees, and more from the Bitcoin network." />
</head>

The `omniTransactions` allows us to fetch details about omni tranasctions from Bitcoin network.

Here is an example that demonstrates `omniTransactions` query:

```
{
  bitcoin {
    omniTransactions(
      options: {limit: 10, desc: "block.timestamp.iso8601"}
      date: {after: "2023-07-22"}
    ) {
      block {
        timestamp {
          iso8601
        }
      }
      blockHash
      feeValue
      hash
      index
      json
      txSender
      type
      typeInt
      valid
      version
    }
  }
}
```

<details>
<summary>Filtering Omni Transactions</summary>

Omni Transactions can be filtered using the following arguments

-   `any`:
-   `date`: Filter by selecting the range, list or just date.
-   `feeValue`: Filter by transaction fee value
-   `height`: Filter by block height
-   `invalidReason`: 
-   `options`: Filter returned data by ordering, limiting, and constraining it.
-   `time`: Filter by selecting time in range, list or just time
-   `txHash`: Filter by transaction hash 
-   `txIndex`: Filter by transaction index in block
-   `txSender`: Filter by address of transaction sender
-   `type`: Filter by type
-   `typeId`: Filter by type Id
-   `valid`:
-   `version`: Filter by version

</details>

The following are available fields for the `omniTransactions`:

-   `any`:
-   `block`: returns block where transaction is included
-   `blockHash`: returns block hash
-   `count`: returns aggregate count of omni transactions
-   `countBigInt`: returns count as `BigInt`
-   `date`: returns date of the transactions
-   `expression`: performs arithematic operation on fields in the query and returns value of the operation
-   `feeValue`: returns transactions total fee value
-   `hash`: returns hash of the transaction
-   `index`: returns index of omni transaction in the block
-   `invalidReason`:
-   `json`: 
-   `maximum`: returns maximum for selected measurable field of Bitcoin Omni Transactions
-   `minimum`: returns minimum for selected measurable field of Bitcoin Omni Transactions
-   `txSender`: returns transaction sender
-   `type`: returns type of transaction
-   `typeInt`: returns type as Int
-   `valid`:
-   `version`: returns version
