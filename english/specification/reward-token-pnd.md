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

# Reward Token (PND)

### Overview of Rewards

PND reward rates are displayed in the red box below on each pool detail page,

with rewards for base asset borrowers as Borrow Reward APR,

and rewards for base asset lenders as Deposit Reward APR.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2Fjc6V6StsCVaGd5jPr4N5%2FGroup%20122.png?alt=media&#x26;token=54036a85-c612-4b81-812a-c46837f3bf1a" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
APR is an abbreviation for Annual Percentage Rate (annualized yield), calculated using simple interest.
{% endhint %}

### Reward Generation and Distribution

When deposits to each pool exceed the threshold, rewards are generated with each Ethereum block,

and distributed to borrowers and lenders according to each pool's supply utilization rate.

Since interest incurred by borrowers is a major factor discouraging borrowing,

punodwoɔ is designed to offset this interest as much as possible with borrow rewards.

### Supply Utilization Rate and Distribution Ratio

A specific supply utilization rate for each pool is set as kink,

with 100% of rewards distributed to borrowers below kink, and rewards generated for lenders after kink.

The "distribution ratio for borrowers and lenders" according to supply utilization rate is displayed at the bottom of each pool detail page.

<figure><img src="../.gitbook/assets/Group 35.png" alt=""><figcaption></figcaption></figure>

### How to Read the Graph

The horizontal axis (X-axis) of the graph represents supply utilization rate, with values from 0% to 100%.

The vertical axis (Y-axis) of the graph represents distribution ratio, with values from 0% to 100%.

The pink line represents the borrower's distribution ratio, and the green line represents the lender's distribution ratio.

Reward APR is calculated using the following formula based on the "distribution ratio for borrowers and lenders" and other factors.

```
a: PND reward amount per block
b: Number of blocks per year (2,628,000 blocks)
c: PND price at that point (obtained from various oracles)
d: Distribution ratio for borrowers and lenders (0% to 100%)
e: Total borrow amount for borrowers, total deposit amount for lenders
Reward APR = a × b × c × d ÷ e × 100
```

When the cursor is not over the graph, various reward APRs based on the current supply utilization rate are displayed on the right,

and when the cursor is over the graph, reward APRs based on the supply utilization rate corresponding to the cursor position are displayed.

### Claiming Rewards

Earned rewards are displayed in the red box below on the pool detail page.

You can claim earned rewards using the Claim button in the blue box.

ETH is required for gas fees, so please prepare it in your wallet.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2Fa0FN1EtqCEwmRoBPqjuT%2FGroup%2029.png?alt=media&#x26;token=4e1e4389-8e9a-4f7a-a290-9d204290e27c" alt=""><figcaption></figcaption></figure>

### Effective APR

The effective deposit APR and effective borrow APR displayed on the pool list are calculated based on interest rate APR and reward APR,

Effective Deposit APR = Deposit APR + Deposit Reward APR

Effective Borrow APR = Borrow APR - Borrow Reward APR.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2FvT7uiP74CmggUY0XBQML%2FGroup%2028.png?alt=media&#x26;token=5665a637-a184-4315-a8e1-e72fd2da2dc5" alt=""><figcaption></figcaption></figure>
