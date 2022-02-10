---
title: {{ replace .Name "-" " " | title }}
date: {{ dateFormat "2006-01-02" .Date }}
draft: true

type: "posts"
hiddenFromHomePage: false

categories: ["art"]
tags: ["sketch"]

summary: >-
  Pencil sketch of {{ replace .Name "-" " " | title }}.

toc: false
images: ["{{ .Name }}.webp"]
---

{{< image src={{ .Name }}.webp caption="{{ replace .Name "-" " " | title }}" height=100% width=100% >}}
