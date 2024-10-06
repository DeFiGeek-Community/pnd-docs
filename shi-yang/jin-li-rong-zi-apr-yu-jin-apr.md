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

# 金利（融資APR、預金APR）

## 金利の概要

金利は、

ベース資産の借り手に対する金利を融資APR、

ベース資産の貸し手に対する金利を預金APRとして、

各プール詳細ページの以下の赤枠の箇所に表示されています。

<figure><img src="../.gitbook/assets/Group 22.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
APRは、Annual Percentage Rate（年換算利回り）の略語で、単利計算です。
{% endhint %}

## 元本と金利

ベース資産を借り入れている時には、元本に金利を掛け合わせた利息と元本が借入額となります。

ベース資産を預け入れている時には、元本に金利を掛け合わせた利息と元本が預金額となります。

## 利息の発生

利息はイーサリアムチェーンのブロックごとに発生しますので、

現在のところおよそ12秒ごとに増加していく計算になります（2024年10月時点）。

## 金利と預金融資率のグラフ

また、融資APRと預金APRは、各プールの預金融資率に連動して増減します。

各プールの詳細ページの最下部の金利APRグラフをご覧ください。

<figure><img src="../.gitbook/assets/スクリーンショット 2024-09-26 20.28.47.png" alt=""><figcaption></figcaption></figure>

## グラフの見方

グラフの横軸（X軸）は預金融資率を表し、0％から100％までの値となります。

グラフの縦軸（Y軸）は金利APRを表し、0％からAPRの最大値までの値となります。

ピンクの直線が融資APR、緑の直線が預金APRを表しています。

「直線の傾き」と「supply kink、borrow kinkと呼ばれる特定の預金融資率」は各プールで設定されており、

kinkを超えると金利の上昇速度が上がり（直線の傾きが急になり）ます。

グラフ上にカーソルが乗っていない時は、現在の預金融資率に基づく各種APRが右側に表示され、&#x20;

グラフ上にカーソルが乗っている時は、カーソル位置に応じた預金融資率に基づくAPRが表示されます。

{% hint style="info" %}
借り手に対する利息は、PND報酬でほぼ相殺できるよう設計されています。\
詳しくは[PND報酬のページ](pndtkun.md)をご覧ください。
{% endhint %}
