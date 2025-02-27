---
description: PND報酬とは
---

# 報酬トークン（PND）

## 報酬の概要

PND報酬率は、

ベース資産の借り手に対する報酬を融資報酬APRとして、

ベース資産の貸し手に対する報酬を預金報酬APRとして、

各プール詳細ページの以下の赤枠の箇所に表示されています。

<figure><img src="../.gitbook/assets/Group 122.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
APRは、Annual Percentage Rate（年換算利回り）の略語で、単利計算です。
{% endhint %}

## 報酬の発生と分配

各プールへの預金額が閾値を上回るとイーサリアムのブロックごとに報酬が発生し、

各プールの預金融資率に応じて、借り手と貸し手に分配されます。

借り手に発生する利息は、借入を控える主要因となるため、

punodwoɔではこの利息を融資報酬で出来るだけ相殺できるように設計しました。

## 預金融資率と分配比率

各プールの特定の預金融資率をkinkとして設定し、

kink未満では借り手に100％報酬が分配され、kink以降に貸し手に報酬が発生するようにしてます。

預金融資率に応じた 「借り手、貸し手の分配比率」 は、各プール詳細ページの最下部に表示されています。

<figure><img src="../.gitbook/assets/Group 27 (1).png" alt=""><figcaption></figcaption></figure>

## グラフの見方

グラフの横軸（X軸）は預金融資率を表し、0％から100％までの値となります。

グラフの縦軸（Y軸）は分配比率を表し、0％から100％までの値となります。

ピンクの直線が借り手の分配比率、緑の直線が貸し手への分配比率を表しています。

報酬APRはこの借り手、貸し手の分配比率」などを元に、以下の計算式で求められます。

```
a : 1ブロックごとのPND報酬量
b : 年間ブロック数（2628000ブロック）
c : 時点のPND価格（各種オラクルより取得）
d : 借り手、貸し手の分配比率（0%〜100%）
e : 借り手の場合は総借入額、貸し手の場合は総預金額
報酬APR = a × b × c × d ÷ e × 100
```

グラフ上にカーソルがない時は、現在の預金融資率に基づく各種報酬APRが右側に表示されており、&#x20;

グラフ上にカーソルがある時は、カーソル位置に応じた預金融資率に基づく報酬APRが表示されます。

## 報酬の請求

獲得した報酬はプール詳細ページの以下の赤枠に表示されます。

また、青枠の請求ボタンで獲得した報酬を請求できます。

ガス代としてETHが必要になりますので、ウォレットにご準備ください。

<figure><img src="../.gitbook/assets/Group 29.png" alt=""><figcaption></figcaption></figure>

## 実質APR

プール一覧に表示されている実質預金APR、実質融資APRは、金利APRと報酬APRを元に、

実質預金APR = 預金APR ＋ 預金報酬APR

実質融資APR = 融資APR - 融資報酬APR　で算出された値です。

<figure><img src="../.gitbook/assets/Group 28.png" alt=""><figcaption></figcaption></figure>
