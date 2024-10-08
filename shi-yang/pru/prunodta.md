---
layout:
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
---

# プールのデータ解説

## 各種データ

一覧には左から、各プールの預金融資率、実質預金APR、実質融資APR、総預金、総融資、担保資産が表示されています。

<figure><img src="../../.gitbook/assets/Group 14_2.png" alt=""><figcaption></figcaption></figure>

## 預金融資率とは

プールに預け入れられた総ベース資産額に占めるベース資産の融資額の割合です。

{% hint style="info" %}
計算式：総融資額 / 総預金額 × 100&#x20;
{% endhint %}

預金融資率の枠にあるドーナツチャートは、supply kink-10%までは緑色、kinkまでは黄色、それ以降は赤色に変化します。

<div align="center" data-full-width="true">

<figure><img src="../../.gitbook/assets/スクリーンショット 2024-07-24 20.58.34.png" alt=""><figcaption></figcaption></figure>

</div>

supply kinkについてはドキュメントの[利息のページ](../jin-li-rong-zi-apr-yu-jin-apr.md)ご覧ください。&#x20;

## 実質預金APR

預金APR + PND報酬APRで算出されています。

## 実質融資APR

&#x20;融資APR - PND報酬APRで計算されます。&#x20;

{% hint style="info" %}
APRは、Annual Percentage Rate（年換算利回り）の略語で、単利計算です。
{% endhint %}

実質預金APR、実質融資APRは共に、預金融資率とPND APRの変化に伴って変動します。&#x20;

## 総預金、総融資、総担保

K（千）やM（百万）で数値を丸めておりますが、\
カーソルを値にホバーすると、実際の価格が表示されます。&#x20;

<figure><img src="../../.gitbook/assets/スクリーンショット 2024-07-25 20.14.23.png" alt=""><figcaption></figcaption></figure>
