---
description: CJPY pool as an example
---

# Background of Reward Speed Determination

The CJPY pool's reward speed was initially 5.2164 PND per day.

This speed was determined to offset base borrow interest with PND rewards.

Specifically, CJPY pool rewards begin to be generated when total borrows exceed 10 million CJPY,

and since the CJPY pool's minimum borrow interest rate is 2.75%, 10 million × 0.0275 = 275,000 (CJPY). This is what all borrowers bear over one year.

To find the daily amount, divide by 365.

275,000 ÷ 365 = 753 (CJPY).

When the reward speed was initially determined, 1 USD = 144.352 JPY and 1 USD = 1 PND was assumed, so

the reward to offset 753 CJPY was set at 753 ÷ 144.352 = <mark style="color:red;">**5.2164**</mark> (PND).

Currently, the initial assumption of 10 million CJPY borrows has increased to approximately 50 million CJPY, 5 times the original,

and considering that the assumed state where PND at $1 assumption can offset base APR is actually trading around $0.01 (1/100),

the reward speed has been adjusted to <mark style="color:red;">**500 times**</mark> the original (5 times × 100 times).

Therefore, it is now 5.2164 × 500 = <mark style="color:red;">**2,608.2**</mark> (PND) per day.

This 2,608.2 PND is shared between borrowers and lenders.

We will continue to adjust the reward speed considering changes in total borrows and PND price.
