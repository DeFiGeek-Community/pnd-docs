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

# 関係式

次の式を満たす場合このアカウントは清算対象となります。\
（あるアカウントの借入額が清算閾値以上かを判別する式）

```
a： ベース資産の借入額
b： 担保価値
c： 清算掛目

a - bc ≧ 0
```

以下の式を満たす場合は清算が正常に行われます。\
（借り手に残る担保資産が0ドル以上かを判別する式）

```
a： 担保価値
b： ベース資産の借入額
c： 清算ペナルティ率

a - b（ 1 + c ） ≧ 0
```
