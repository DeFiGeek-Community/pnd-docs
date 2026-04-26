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

# Interest Rates (Borrow APR, Deposit APR)

### Overview of Interest Rates

Interest rates are displayed in the red box below on each pool detail page,

with interest rates for base asset borrowers as Borrow APR,

and interest rates for base asset lenders as Deposit APR.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2FPTGxeVhEnqlUdyMQ3t4p%2FGroup%2022.png?alt=media&#x26;token=e6db805f-f118-45f3-9ebd-28e93a70b083" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
APR is an abbreviation for Annual Percentage Rate (annualized yield), calculated using simple interest.
{% endhint %}

### Principal and Interest

When borrowing base assets, interest calculated by multiplying principal by the interest rate plus principal becomes the borrow amount.

When depositing base assets, interest calculated by multiplying principal by the interest rate plus principal becomes the deposit amount.

### Interest Accrual

Interest accrues with each Ethereum block,

so currently it increases approximately every 12 seconds (as of October 2024).

### Interest Rate and Supply Utilization Rate Graph

Borrow APR and Deposit APR also increase and decrease in response to each pool's supply utilization rate.

Please see the interest rate APR graph at the bottom of each pool's detail page.

<figure><img src="https://3990862584-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FKP6SsdesCFe6jfgBhMAY%2Fuploads%2FoJHcVSS4Ot6ctYqxH6Le%2F%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%BC%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%83%E3%83%88%202024-09-26%2020.28.47.png?alt=media&#x26;token=032134e1-d1bc-4f0d-b2c9-19598a800c81" alt=""><figcaption></figcaption></figure>

### How to Read the Graph

The horizontal axis (X-axis) of the graph represents supply utilization rate, with values from 0% to 100%.

The vertical axis (Y-axis) of the graph represents interest rate APR, with values from 0% to the maximum APR.

The pink line represents Borrow APR, and the green line represents Deposit APR.

The "slope of the line" and "specific supply utilization rates called supply kink and borrow kink" are set for each pool,

and when kink is exceeded, the interest rate increase speed rises (the line slope becomes steeper).

When the cursor is not over the graph, various APRs based on the current supply utilization rate are displayed on the right,

and when the cursor is over the graph, APRs based on the supply utilization rate corresponding to the cursor position are displayed.

{% hint style="info" %}
Interest for borrowers is designed to be largely offset by PND rewards.\
For details, please see the [PND rewards page](https://pnd-docs.defigeek.xyz/shi-yang/tkunpnd).
{% endhint %}
