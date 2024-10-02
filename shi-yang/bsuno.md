---
description: ベース資産の借入の解説
---

# ベース資産の借入

各プールに各ユーザーのベース資産の借入可能枠があり、担保を入れていない状態ではこの枠は0です。

<figure><img src="../.gitbook/assets/Group 20a (1).png" alt=""><figcaption></figcaption></figure>

ユーザーがプールに担保資産を預け入れると、米ドルベースの担保価値に担保掛目が掛け合わされ、\
その額だけベース資産の借入可能枠が増加します。

例えば、担保掛目80の担保を時価100ドル分預け入れると、

100 × 0.80 = 80（ドル）

80ドル分の枠が増え、80ドル分のベース資産を借り入れることが可能になります。

<figure><img src="../.gitbook/assets/Group 20.png" alt=""><figcaption></figcaption></figure>

担保掛目は各プールの各担保資産に固有の値を割り当てておりますので、\
プール詳細ページでご確認ください。

<figure><img src="../.gitbook/assets/Group 13_1.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
ボラティリティ（価格変動）が大きい担保を預け入れている場合、時事刻々と増減する借入可能枠の変動も大きくなりますので、ご承知おき下さい。
{% endhint %}

ベース資産を借り入れると、融資利息と報酬が発生いたします。

融資利息は、元本と共に債務となります。

融資金利は、プール詳細ページに融資APRとして記載しております。

また、報酬はPNDトークンで、報酬率はプール詳細ページの融資APRの下に記載しております。

併せてご確認ください。

<figure><img src="../.gitbook/assets/Group 13_2.png" alt=""><figcaption></figcaption></figure>
