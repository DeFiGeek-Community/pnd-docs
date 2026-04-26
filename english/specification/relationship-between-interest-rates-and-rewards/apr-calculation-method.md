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

# APR Calculation Method

The vertical axis of all graphs in punodwoɔ represents APR (annualized yield).

APR for borrowers and lenders is calculated using the following formulas respectively.

```
Annualized reward amount for borrowers = baseTrackingBorrowSpeed / 10^15 × 60 × 60 × 24 × 365 × PND unit price
Borrow Reward APR = Annualized reward amount for borrowers / Total borrows × 100
```

```
Annualized reward amount for lenders = baseTrackingSupplySpeed / 10^15 × 60 × 60 × 24 × 365 × PND unit price
Deposit Reward APR = Annualized reward amount for lenders / Total deposits × 100
```

APR <mark style="color:red;">changes</mark> due to fluctuations in the variables in the above formulas (baseTrackingRewardSpeed for borrows and deposits for any pool, total amounts, and PND unit price).

Conversely, the values shown in the graphs are the values assuming these variables remain at current levels for one year without deviation.

By multiplying APR by your borrowed or deposited base assets, you can calculate interest or rewards under the above assumption.

When the CJPY pool's interest rate APR for borrowers is 4.109% and reward APR is 0.543%,\
effective borrow APR is 4.109 - 0.543 = 3.566%, and borrow interest is incurred.\
When the above variables fluctuate and interest rate APR and reward APR become equal, <mark style="color:red;">when effective borrow APR becomes 0%,</mark>

<mark style="color:red;">the state where interest is offset by rewards</mark> is achieved.
