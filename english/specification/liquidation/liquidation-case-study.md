---
description: TXJP from punodwoɔ’s CJPY pool as an example
---

# Liquidation Case Study

### Collateral Parameters (Example: TXJP in CJPY Pool)

Collateral Factor: 80%, Liquidation Threshold Factor: 90%, Liquidation Penalty: 10%

### Account Status at a Certain Point

Collateral value at this point: $100\
Liquidation threshold at this point: $90\
Base asset borrow amount at this point: $80 (borrow limit (capacity))\
Liquidation penalty amount: 80 × 0.10 = $8\
Total repayment amount: 80 + 8 = $88\
Remaining collateral: 90 - 88 = $2\
(Interest and gas fees are not considered)

{% hint style="info" %}
The main cases of liquidation are when collateral value declines or base asset value rises, and\
in reality, both occur simultaneously causing liquidation. However, since it is difficult to grasp the relationship between two constantly fluctuating variables (collateral value and base asset value), the following explanation fixes one of them to make it easier to understand.
{% endhint %}

### Case Studies

1. When Collateral Value Declines (Base Asset Value Fixed at $80)\
   \
   a) Case where liquidation executes normally (borrower's debt can be fully repaid and liquidation penalty is fully covered)\
   　\
   　Example) Liquidation occurs when collateral value drops to $88\
   　　　Liquidation threshold: $79.2\
   　　　Collateral value at that point: $88\
   　　　Liquidation penalty: 80 × 0.10 = $8\
   　　　Total repayment amount: 80 + 8 = $88\
   　　　Collateral remaining for borrower: 88 - 88 = $0\
   \
   b) Case where liquidation does not execute normally (borrower's debt can be fully repaid, but liquidation penalty is insufficient)\
   \
   　Example) Liquidation occurs when collateral value drops to $83\
   　　　Liquidation threshold: $74.7\
   　　　Collateral value at that point: $83\
   　　　Liquidation penalty: 80 × 0.10 = $8\
   　　　Total repayment amount: 80 + 8 = $88 (exceeds collateral value. Shortfall is $5)\
   　　　Collateral remaining for borrower: $0\
   \
   c) Case where liquidation does not execute normally (borrower's debt cannot be fully repaid and liquidation penalty is also insufficient)\
   \
   　Example) Liquidation occurs when collateral value drops to $78\
   　　　Liquidation threshold: $70.2\
   　　　Collateral value at that point: $78\
   　　　Liquidation penalty: 80 × 0.10 = $8\
   　　　Total repayment amount: 80 + 8 = $88 (exceeds collateral value. Shortfall is $8)\
   　　　Collateral remaining for borrower: $0<br>
2. When Base Asset Value Rises (Collateral Value Fixed at $100)\
   \
   a) Case where liquidation executes normally (borrower's debt can be fully repaid and liquidation penalty is fully covered)\
   \
   　Example) Borrower's base asset borrows rise to $90 and liquidation occurs\
   　　　(If base assets are stablecoins, it is unlikely to rise this much in reality)\
   　　　Borrower's base asset borrows: $90\
   　　　Liquidation threshold: $90\
   　　　Collateral value at that point: $100\
   　　　Liquidation penalty: 90 × 0.10 = $9\
   　　　Total repayment amount: 90 + 9 = $99\
   　　　Collateral remaining for borrower: 100 - 99 = $1\
   \
   b) Case where liquidation does not execute normally (borrower's debt can be fully repaid, but liquidation penalty is insufficient)\
   \
   　Example) Case where borrower's base asset borrows rise to $95 and liquidation occurs\
   　　　(Case where liquidation is easily skipped because full liquidation penalty cannot be obtained)\
   　　　Borrower's base asset borrows: $95\
   　　　Liquidation threshold: $90\
   　　　Collateral value at that point: $100\
   　　　Liquidation penalty: 95 × 0.10 = $9.5\
   　　　Total repayment amount: 95 + 9.5 = $104.5 (exceeds collateral value. Shortfall is $4.5)\
   　　　Collateral remaining for borrower: $0\
   \
   c) Case where liquidation does not execute normally (borrower's debt cannot be fully repaid and liquidation penalty is also insufficient)\
   \
   　Example) Case where borrower's base asset borrows rise to $100 and liquidation occurs\
   　　　(Case where even if liquidated, liquidator receives no reward and becomes bad debt)\
   　　　Borrower's base asset borrows: $100\
   　　　Liquidation threshold: $90\
   　　　Collateral value at that point: $100\
   　　　Liquidation penalty: 100 × 0.10 = $10\
   　　　Total repayment amount: 100 + 10 = $110 (exceeds collateral value. Shortfall is $10)\
   　　　Collateral remaining for borrower: $0
