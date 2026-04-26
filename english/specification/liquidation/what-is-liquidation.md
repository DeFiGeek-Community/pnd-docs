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

# What is Liquidation

### Liquidation Threshold

When a user deposits collateral assets into the protocol, the liquidation threshold is calculated using the following formula.

{% hint style="info" %}
Liquidation Threshold = Collateral Value × Liquidation Threshold Factor\
Liquidation threshold factors are set for each collateral asset in each pool and can be confirmed on the pool detail page.\
![](https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2FVtDkMxLpvU88gp4q7PxK%2FGroup%2020b.png?alt=media\&token=854ddc68-6a25-4811-ac43-5efb19c6d2d0)
{% endhint %}

For example, if you deposit $100 worth of collateral with a liquidation threshold factor of 90%, the liquidation threshold is 100 × 0.90 = 90 (USD).

The borrower's base asset borrows must be below this liquidation threshold.

{% hint style="info" %}
The liquidation threshold is displayed in the red box on the pool detail page below.\
![](https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2FnrZm6MV5sxsdr5ed1nv4%2FGroup%2020c.png?alt=media\&token=ada3d0ad-9d71-4166-bc98-a200005faa82)
{% endhint %}

### Conditions for Liquidation

However, due to a decline in collateral value or an increase in base asset value, base asset borrows may exceed the liquidation threshold.

{% hint style="info" %}
Since collateral value and base asset value are constantly fluctuating, the liquidation threshold is also constantly rising and falling.
{% endhint %}

### Execution of Liquidation

At this point, anyone can liquidate this borrower's position.

{% hint style="info" %}
Third parties who execute liquidation are called liquidators.\
Liquidators mainly include bots, users, and contracts.
{% endhint %}

When liquidation is executed, the borrower's collateral is confiscated, and in return, the base asset borrows are repaid.

What remains for the borrower is the remaining collateral assets after subtracting the base assets and liquidation penalty.

The liquidation penalty is split between the liquidator and the protocol.

Confiscated collateral assets may be purchased at a discount.
