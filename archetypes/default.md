---
draft: true
title: "page-title"
date: '{{ now.Format "2006-01-02" }}'
showDate: true
url: 'no/id/pm/{{ template "permanentId" }}/'
aliases: '/aliases/{{ template "permanentId" }}/'
categories: ["article",]
tags: [""]
series: [""]
featureimage: ""
series_order: 
showTableOfContents: false
showAuthor: false
---
{{< katex >}}
{{< robot-ignore >}}
![text](img/feature-blog.png)

{{- define "permanentId" -}}
  {{- $scratch := newScratch -}}
  {{- range (seq 10) -}}
    {{- $nextCh := slice "0" "1" "2" "3" "4" "5" "6" "7" "8" "9" "a" "b" "c" "d" "e" "f" "g" "h" "i" "j" "k" "l" "m" "n" "o" "p" "q" "r" "s" "t" "u" "v" "w" "x" "y" "z" | shuffle | first 1 -}}
    {{- $scratch.Add "id" $nextCh -}}
  {{- end -}}
  {{- delimit ($scratch.Get "id") "" -}}
{{- end -}}
