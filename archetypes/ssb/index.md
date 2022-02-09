---
weight: 0

title: "{{ replace .Name "-" " " | title }}"
date: {{ dateFormat "2006-01-02" .Date }}
draft: true

type: "posts"
hiddenFromHomePage: false

categories: ["ssb-stories"]
tags: ["SSB"]

summary: >-
  ""

featuredImage: "/images/{{ .Name }}.webp"
images: "/images/{{ .Name }}.webp"
---
