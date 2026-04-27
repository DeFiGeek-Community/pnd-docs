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

# Pool Data Explanation

### Various Data

The list displays, from left to right, each pool's supply utilization rate, effective deposit APR, effective borrow APR, total deposits, total borrows, and collateral assets.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2FjyuKKB1iFRdSWXoRulHK%2FGroup%2014_2.png?alt=media&#x26;token=36f60770-79a3-4e84-ae8e-a79cb31e7eda" alt=""><figcaption></figcaption></figure>

### What is Supply Utilization Rate

This is the ratio of base asset borrows to the total base assets deposited in the pool.

{% hint style="info" %}
Formula: Total Borrows / Total Deposits × 100
{% endhint %}

The donut chart in the supply utilization rate section changes to green up to supply kink - 10%, yellow up to kink, and red thereafter.

<div align="center" data-full-width="true"><figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2FDPwKKofMShN9CzwRZCJo%2F%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%BC%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%83%E3%83%88%202024-07-24%2020.58.34.png?alt=media&#x26;token=f9c34bd0-254b-4816-b81c-6c1e9f3a2a20" alt=""><figcaption></figcaption></figure></div>

For supply kink, please see the [interest rates page](../interest-rates-borrow-apr-deposit-apr.md) in the documentation.

### Effective Deposit APR

Calculated as Deposit APR + PND Reward APR.

### Effective Borrow APR

Calculated as Borrow APR - PND Reward APR.

{% hint style="info" %}
APR is an abbreviation for Annual Percentage Rate (annualized yield), calculated using simple interest.
{% endhint %}

Both effective deposit APR and effective borrow APR fluctuate according to changes in supply utilization rate and PND APR.

### Total Deposits, Total Borrows, Total Collateral

Values are rounded using K (thousands) or M (millions), but hovering over the value displays the actual price.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2F1EzPPrhMaDkNXrKTW5MZ%2F%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%BC%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%83%E3%83%88%202024-07-25%2020.14.23.png?alt=media&#x26;token=a9112350-0cec-44c1-ba1f-819a2cedd192" alt=""><figcaption></figcaption></figure>
