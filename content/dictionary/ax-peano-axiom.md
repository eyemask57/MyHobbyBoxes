---
title: "Peano の公理"
date: '2025-12-08'
url: 'id/olsce9zcz2/'
aliases: "/aliases/peano-axiom/"
categories: ["数学","集合論","数の構成"]
tags: ["自然数","Peano構造"]
types: [
  "dictionary"
]
showTableOfContents: false
---
{{< katex >}}

### 公理: Peano の公理 [[id/olsce9zcz2/]](id/olsce9zcz2/)

集合 \(\bm{N}\) ，要素 \(0 \in \bm{N}\) ，写像 \(s: \bm{N} \to \bm{N}\) の組 \((\bm{N},0,s)\) について，以下の公理系を **Peano の公理 (Peano axioms)** という．

1. 写像 \(s\) は単射である．
2. \(0 \notin s[\bm{N}] = \set{s(n) | n \in \bm{N}}\) である．
3. 任意の \(A \subset \bm{N}\) について，\(0 \in A,\ s[A] \subset A\) を満たすならば， \(A = \bm{N}\) である．

なお，写像 \(s\) は **後者関数 (successor function)** と言われる．

また，組 \((\bm{N},0,s)\) で， Peano の公理を満たすものを **Peano システム (Peano system)** という．
