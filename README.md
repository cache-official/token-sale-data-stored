# Cache Token Sale Data Transparency

For full transparency we have pasted the type of data that we store for transactions. Most of this information is available on public blockchains and other meta data is only meaningful to the parties involved the transaction. No personal data is saved.

We store transaction data to effectively solve problems with transactions.

**We collect NO data outside of what you see here**

### Coinbase Data
This is the type of data that is stored for Coinbase transactions.

Please note that *addresses* are NOT your Coinbase addresses, these are unique addresses
generated for the specific transaction - the addresses you send crypto to.

```json
{
  "data": {
    "addresses": {
      "ethereum": "0x1d5b1540c1d22cadb437581a2968fe336741e39e",
      "bitcoin": "16QRwkDmdaLGA54AnmiuAqNWGBXh8cnkNM",
      "bitcoincash": "qz1gwkjk8zefx8fmr07gx5wxf42tb87lky9t6qmzay",
      "litecoin": "LPXbearNZ7RVzhfPiBkrzu8vZK6p4b2PnU"
    },
    "code": "ZLV4BXX3",
    "created_at": "2018-05-28T06:43:18Z",
    "expires_at": "2018-05-28T06:58:18Z",
    "hosted_url": "https://commerce.coinbase.com/charges/ZLV4BXX3",
    "metadata": {
      "cache_product_id": "5b07b20f06d7eb88fe233eb3",
      "sender_cache_address": "TBIUQMOGHUH7GN5LM62CQ5CI4JEXMWU455IPHIYZ"
    },
    "name": "Cache Tokens",
    "payments": [],
    "pricing": {
      "local": {
        "amount": "900.00",
        "currency": "USD"
      },
      "ethereum": {
        "amount": "1.706501000",
        "currency": "ETH"
      },
      "bitcoin": {
        "amount": "0.12499991",
        "currency": "BTC"
      },
      "bitcoincash": {
        "amount": "0.96715956",
        "currency": "BCH"
      },
      "litecoin": {
        "amount": "7.92114064",
        "currency": "LTC"
      }
    },
    "pricing_type": "fixed_price",
    "timeline": [
      {
        "status": "NEW",
        "time": "2018-05-28T06:43:18Z"
      }
    ]
  },
  "_id": "5b0ba506f1f32ca3a24e2c1c"
}
```

### XEM Data

Minimal data is collected on XEM transactions.

```typescript
{
	_id: ObjectID;
	senderCacheAddress: string;
	tokenType: TokenType;
	productId?: ObjectID;
	usdPaid?: number;
	quotedAmount?: number;
	totalPaid: number;
	transactionCompletedTimestamp?: string;
	message?: string;
	errMsg?: string;
	createdAt: Date;
}
```

