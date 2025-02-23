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

# APRの算出方法

punodwoɔの全てのグラフの縦軸は、APR（年換算利回り）を表しています。&#x20;

借り手、貸し手へのAPRはそれぞれ以下の式で求まります。

```
借り手への年換算報酬額 ＝ baseTrackingBorrowSpeed / 10^15 × 60 × 60 × 24 × 365 × PND単価
融資報酬APR　＝　借り手への年換算報酬額　/　借入総額　×　100
```

```
貸し手への年換算報酬額 ＝ baseTrackingSupplySpeed / 10^15 × 60 × 60 × 24 × 365 × PND単価
預入報酬APR　＝　貸し手への年換算報酬額　/　貸出総額　×　100
```

以上の式内の変数（任意のプールの貸し借りそれぞれのbaseTrackingRewardSpeedと総額、および

PND単価）の変動により、<mark style="color:red;">APRは変化</mark>します。

&#x20;逆に、それらの変数が１年間現在の数値でブレないと仮定した時の値が、グラフに示されています。

ご自身の借りられている、もしくは、預けているベース資産にAPRを掛け合わせれば、

上記の仮定での金利や報酬を算出できます。&#x20;

CJPYプールの借り手に対する金利APRが4.109%で、報酬APRが0.543%の場合、&#x20;

実質融資APRは4.109 - 0.543 = 3.566%で、借入金利が発生します。&#x20;

上記の変数が変動し、金利APRと報酬APRが等しくなり、<mark style="color:red;">実質融資APRが0%となった時に、</mark>&#x20;

<mark style="color:red;">金利を報酬で相殺できた状態</mark>となります。
