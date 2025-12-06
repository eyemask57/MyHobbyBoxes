---
draft: true
title: "距離に触れてみよう"
date: '2025-12-02'
url: 'pm/hxm5rsea2b/'
categories: ["数学","幾何学"]
tags: ["距離空間","距離","位相空間論","位相幾何学"]
series: ["距離空間"]
series_order: 1
types: ["article"]
toc: false
---
{{< katex >}}

## 1. Euclid距離

数学をちょっと学ぶと，僕たちはよく **Euclid 空間** に住んでいると言われることがある．\
まぁ実際は相対論的に考えて違うらしいが，そう考えて差し支えない状況がほとんどである．

そして，そこで距離と言われているのは特に **Euclid 距離** のことである．\
名前は少し怖いが，二点の間の直線距離のことである．一番直観的でわかりやすい距離．

---

### 定義: Euclid 距離 [[/id/m3nsu3isaf/]](/id/m3nsu3isaf/)

\(x,y\)を \(n\) 次元 Euclid空間 \(\mathbb{R}^n\)
(\(\mathrm{i.e.} \ x,y \in \mathbb{R}^n\)) の元とする．\
また，\(x_i,y_i\) を \(x,y\) の \(i\) 成分 (\(i = 1,2,\ldots,n\)) とする．

このとき，**Euclid 距離 (Euclidian distance)** \(d_n(x,y)\) を
\[
    \displaystyle d_n(x,y)
    \coloneqq \sqrt{\sum^n_{i=1} x_i y_i}
    = \sqrt{x_1 y_1 + x_2 y_2 + \cdots + x_n y_n}
\]
と定義する．

---

ちなみに，高校のときの書き方は \(\vec{x},\vec{y}\) とはあまり書かない．\
別に書いてもいいが，なんとなくダサさを感じるし，めんどくさい．

また，物理と違って数学ではベクトルを太字にすることが少ない．\
つまり \(\bm{x},\bm{y}\) とはあまり書かない，かなぁ．
もちろんそう書いてもいい．

---

しかし，実は距離と呼べるもの，間を考えるときに使う道具はこれだけではない．

## n. 一般の距離

---

### 定義: 距離(metric) [[/id/lk9nht7x48/]](/id/lk9nht7x48/)

集合 \(X\) の **距離(metric)** または **距離関数(metric function)**
は以下の公理を満たす写像
\( d : X \times X \to \mathbb{R} \)
である．

1. 任意の \(x,y \in X\) について， \(d(x,y) = 0 \iff x = y\)
2. 任意の \(x,y \in X\) について， \(d(x,y) = d(y,x)\)
3. 任意の \(x,y,z \in X\) について， \(d(x,y) + d(y,z) \ge d(x,z)\)

---
