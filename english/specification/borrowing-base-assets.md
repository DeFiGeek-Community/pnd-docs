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

# Borrowing Base Assets

### Borrow Capacity

Each pool has a borrow capacity for each user's base assets, which is 0 when no collateral is deposited.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2F0wpZpedFOC5QTrik8Qzs%2FGroup%2020a.png?alt=media&#x26;token=25c2beb9-482e-41b3-aaa6-02144c73790c" alt=""><figcaption></figcaption></figure>

### Expanding Borrow Capacity

When a user deposits collateral assets into a pool, the collateral value in USD is multiplied by the collateral factor, and the borrow capacity for base assets increases by that amount.

For example, if you deposit $100 worth of collateral with a collateral factor of 80,

100 × 0.80 = 80 (USD)

The capacity increases by $80, allowing you to borrow $80 worth of base assets.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2FXR2mtWKjtJJvcrWGRNN8%2FGroup%2020.png?alt=media&#x26;token=c131b446-663a-4ba6-b11b-dd28050edd4c" alt=""><figcaption></figcaption></figure>

### How to Read Collateral Factor

Collateral factors are assigned unique values for each collateral asset in each pool, so please check the pool detail page.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2F3dU8jJa35wBo4qFq2upn%2FGroup%2013_1.png?alt=media&#x26;token=7b81ac75-f0e9-40a4-941b-43e6208d90ec" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Please note that when depositing collateral with high volatility (price fluctuations), the fluctuations in borrow capacity that increase and decrease moment by moment will also be larger.
{% endhint %}

### Interest and Rewards

When you borrow base assets, borrow interest and rewards are generated.

Borrow interest becomes debt along with principal.

Borrow interest rates are displayed as Borrow APR on the pool detail page.

Rewards are in PND, and the reward rate is displayed below Borrow APR on the pool detail page.

Please check both.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2FN5EMOfHEo4Y9AINMFyHq%2FGroup%2013_2.png?alt=media&#x26;token=85562598-275a-4145-a53b-23546eb2274d" alt=""><figcaption></figcaption></figure>
