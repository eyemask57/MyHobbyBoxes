---
title: "命題: 自然数の正当性"
date: '2025-12-08'
url: 'id/lyby0a3r5y/'
aliases: "/aliases/prop-natural-number/"
categories: ["数学","集合論","数の構成"]
tags: ["自然数","Peano の公理"]
showTableOfContents: false
showAuthor: false
---
{{< katex >}}

### 命題: 自然数の正当性 [[/id/lyby0a3r5y/]](/id/lyby0a3r5y/)

組 \((\bm{N},0,s)\) について，以下のように定義する．

- [最小の帰納的集合](/id/w7xfgw3xik/) \(\bm{N} \coloneqq \mathbb{N}\)
- \(0\coloneqq \emptyset \in \bm{N}\)
- \(s: \bm{N} \to \bm{N}; s(n) = n \cup \{n\}\)

このとき，組 \((\bm{N},0,s)\) は [Peano システム](/id/olsce9zcz2/)である．

### 証明 [/id/lyby0a3r5y/]

組 \((\bm{N},0,s)\) が Peano システムの全ての性質を持つことを示す．

#### 補題 1

\(n \in s(n),\ n \neq s(n)\) から \(0 \notin s[\bm{N}] = \set{s(n)|n \in \bm{N}}\) である．\(\quad\square\)

#### 補題 2

\(\bm{N}\) の部分集合 \(A\) が \(0 \in A,\ s[A] = \set{s(a) | a \in A} \subset A\) を満たすとき， \(n \in A\) ならば \(n \cup \{n\} = s(n) \in A\) より， \(A\) は帰納的集合である．

\(A\) の部分集合で帰納的集合であるものすべての共通部分を \(\mathbb{N}_A\) とする．
**「定義: 最小の帰納的集合 [[/id/w7xfgw3xik/]](id)」** より \(\mathbb{N}_A = \mathbb{N} = \bm{N}\)．

よって，\(\bm{N} \subset A,\ A \subset \bm{N}\) より \(A = \bm{N}\)．\(\quad\square\)

#### 補題 3

\(s(n)\) は単射であることを示す．

- **方針:** 任意の \(n,m \in \bm{N}\) について，以下を示す．最後の式は単射の定義である．
  1. \(n \in m \implies n \subset m\)
  2. \(s(m) \subset s(n) \implies m \subset n\)
  3. \(s(m) = s(n) \implies m = n\)

##### **補題 3-1**

[補題 2](#補題-2) より，任意の \(n \in \bm{N}\) について，
\[
  A_n \coloneqq \set{m \in \bm{N} | n \in m \implies n \subset m}
\]
より，\(0 \in A_n ,\ s[A_n] \subset A_n \implies A_n = \bm{N}\) ，つまり任意の \(n,m \in \bm{N}\) について \(n \in m \implies n \subset m\) が成り立つことを示す．

任意の \(n \in \bm{N}\) について \(n \notin 0\) より，
\(n \in 0 \implies n \subset 0\) は真である．
よって， \(0 \in A_n\) である．

任意の \(m \in A_n\) について
\[
  s(m) \in A_n \iff [n \in s(m) \implies n \subset s(m)]
\]
であることを示す．
\(n \in s(m) = m \cup \{m\}\) より， \(n \in m\) または \(n = m\) である．

1. \(n \in m\) のとき，前提の \(m \in A_n\) より \(n \subset m\) ，よって \(m \subset s(m)\) から \(n \subset s(m)\)．
2. \(n = m\) なら， \(m \subset s(m)\) より \(n \subset s(m)\)．

よって，任意の \(n,m \in \bm{N}\) について \(n \in m \implies n \subset m\) である．\(\quad\square\)

##### **補題 3-2**

\(s(m) \subset s(n) \) であるとする．また，\(a \in \bm{N}\) について，\(a \in a \cup \{a\} = s(a)\) である．

[補題 3-1](#補題-3-1) より，各 \(n,m \in \bm{N}\) について，

- \(n \in s(n),\ s(n) \subset s(m)\) より， \(n \in s(m)\)．
- \(s(m) = m\cup\{m\}\) より， \(n \subset m\) または \(n = m\)．
- \(n = m \implies n \subset m\)．

よって，任意の \(n,m \in \bm{N}\) について \(s(m) \subset s(n) \implies m \subset n\) である．\(\quad\square\)

##### **系 3-3**

\(s(n) = s(m)\) であるとする．

仮定より \(s(n) \subset s(m),\ s(m) \subset s(n)\)である．
[補題 3-2](#補題-3-2) より \(n \subset m,\ m \subset n\)なので \(n = m\) である．

よって，任意の \(n,m \in \bm{N}\) について \(s(m) = s(n) \implies m = n\) である．\(\quad\square\)

[系 3-3](#系-3-3) より， 写像 \(s\) は単射である．\(\quad\square\)

[補題 1](#補題-1)，[補題 2](#補題-2)，[補題 3](#補題-3) より，組 \((\bm{N},0,s)\) は Peano システムである．\(\quad\square\)
