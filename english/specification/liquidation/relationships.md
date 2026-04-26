---
layout:
  width: default
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
---

# Relationships

An account becomes eligible for liquidation when the following formula is satisfied.\
(Formula to determine if an account's borrow amount is at or above the liquidation threshold)

```
a: Base asset borrow amount
b: Collateral value
c: Liquidation threshold factor

a - bc ≧ 0
```

Liquidation executes normally when the following formula is satisfied.\
(Formula to determine if collateral assets remaining for the borrower are $0 or more)

```
a: Collateral value
b: Base asset borrow amount
c: Liquidation penalty rate

a - b(1 + c) ≧ 0
```
