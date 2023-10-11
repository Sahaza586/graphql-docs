---
title: Algorand Coinpath API
description: Explore money flow in the Algorand blockchain with the Coinpath API, offering detailed insights and advanced filters like currency, date, and more.
image: /img/social-preview/algorand-social.png
keywords: [algorand, algorand crypto, algorand explorer, algorand nft, algorand stats, algorand tvl, algorand staking, algorand block explorer]
---

The Coinpath API allows us to retrieve detailed information about money flow using coinpath technology from Algorand.

<details>
<summary>Filtering Options</summary>

Coinpath data can be filtered using following arguments:

- `currency`: Filter by the currency involved in the transaction.
- `date`: Filter by the date of the transaction.
- `depth`: Filter by the depth of the transaction.
- `initialAddress`: Filter by the initial address.
- `initialDate`: Filter by the initial date.
- `initialTime`: Filter by the initial time.
- `options`: Filter returned data by ordering, limiting, and constraining it.
- `receiver`: Filter by the receiver's address.
- `sender`: Filter by the sender's address.
- `time`: Filter by the time of the transaction.
  
</details>

The following are available fields for the `coinpath`:

- `amount`: returns the amount of tokens involved in the transaction.
- `any`:
- `block`: returns details of the block where the transaction happened.
- `count`: returns the aggregate count of transactions.
- `countBigInt`: returns the aggregate count of transactions in BigInt format.
- `currency`: returns details of the currency used in the transaction.
- `depth`: returns depth information.
- `maximum`: returns maximum of selected [coinpath measurable fields](/v1/docs/graphql-reference/enums/coinpath-measureable)
- `minimum`: returns minimum of selected [coinpath measurable fields](/v1/docs/graphql-reference/enums/coinpath-measureable)
- `receiver`: returns information about the receiver.
- `sender`: returns information about the sender.
- `transaction`:  returns transaction details.
- `transactions`: returns attributes of transactions.