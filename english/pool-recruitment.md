---
description: Application Guidelines
---

# Pool Recruitment

We offer free pool deployment services for those who wish to use specific base (lending) assets or collateral assets.

### Use Cases

When you need permissionless lending for crypto assets not supported by other lending protocols, you can operate lending pools on punodwoɔ's proven track record and security.

### Items Requiring Prior Decision by the Requester

1. Token type for base assets (Ethereum mainnet)
2. Token types for collateral assets (maximum 15 types, Ethereum mainnet)
3. Collateral factor, liquidation threshold, liquidation penalty, and supply cap for each collateral asset
4. Price feed instructions for each token (DEX TWAP, ChainLink, etc.)
5. Interest rate curve settings for supply and borrow sides (low rate, kink, high rate)
6. Reward settings (set PND distribution flow rate. PND must be procured by the requester from the market.)
7. Threshold deposit amount for reward generation

### Notes

* Regarding item 3 above: The liquidation threshold and liquidation penalty must be set together to 100 or less.
* Regarding item 3 above: Supply cap refers to the token supply limit. This is the total amount of collateral tokens that can be deposited into punodwoɔ as collateral. Limiting the acceptance amount as collateral enhances protocol security and benefits users. For high market cap tokens, approximately 1% of circulating supply is recommended, and for low market cap tokens, approximately 10% of circulating supply is recommended.
* Regarding item 5 above: For the borrow side, it is important to determine the base rate (base interest rate at minimum utilization). It is recommended to set this using a simulator to ensure the protocol does not operate at a loss. Please refer to [this](https://docs.google.com/spreadsheets/d/11nsgJ6tvmC3y81_NqqqwU4Kv9mzkBIooC7QqESWMx4U/edit?gid=1000488205#gid=1000488205) as a reference. The protocol accumulates reserves through the difference between lending and borrowing interest rates, enabling more autonomous and sustainable operations. Reserves can also be used as a source of profit distribution.

### Fees

After sharing the above decisions with DFGC, DFGC will deploy the pool contracts at no cost. Updates such as parameter changes or asset additions will be at the requester's expense.

### Contact

DFGC Development Team will provide full support, so please feel free to contact us with any questions or requests.\
Please contact us through the Discord community below.\
[https://discord.com/channels/705052448418693180/1167369964286652436](https://discord.com/channels/705052448418693180/1167369964286652436)

english general channel:\
[https://discord.com/channels/705052448418693180/705290863353397338](https://discord.com/channels/705052448418693180/705290863353397338)
