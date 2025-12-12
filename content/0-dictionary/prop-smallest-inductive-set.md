---
title: "命題: 最小の帰納的集合の一意性"
date: '2025-12-08'
url: 'id/2v3gcmrrcp/'
aliases: "/aliases/prop-inductive-set/"
categories: ["数学","集合論","数の構成"]
tags: ["自然数","Peano の公理"]
showTableOfContents: false
showAuthor: false
---
{{< katex >}}

### 命題: 最小の帰納的集合の一意性 [[/id/2v3gcmrrcp/]](/id/2v3gcmrrcp/)

帰納的集合 \(A\) の部分集合で帰納的集合であるものすべての共通部分を \(\mathbb{N}_A\) とする．

このとき，任意の帰納的集合 \(X,Y\) について，\(\mathbb{N}_X=\mathbb{N}_Y\) である．

### 証明．[/id/2v3gcmrrcp/]

- **方針:** \(Y\) の帰納的な部分集合をとり，\(\mathbb{N}_X \subset \mathbb{N}_Y\) を示す．対称性より片方のみで十分．

任意の帰納的な部分集合 \(A \subset Y\) をとる．

\(A,X\) は定義より空集合を要素として含み，またどちらも帰納的集合であるため，\(A \cap X\) も帰納的である．

\(A \cap X \subset X\) であり， \(\mathbb{N}_X\) の定義より \(\mathbb{N}_X \subset A \cap X\) である．
\(A \cap X \subset A\) より \(\mathbb{N}_X \subset A\)，
\(A\) は \(Y\) の任意の帰納的な部分集合であるので，\(A = \mathbb{N}_Y\) として \(\mathbb{N}_X \subset \mathbb{N}_Y\)である．

対称性より \(\mathbb{N}_Y \subset \mathbb{N}_X\) も同様であるため，\(\mathbb{N}_X = \mathbb{N}_Y\)．\(\quad\square\)
