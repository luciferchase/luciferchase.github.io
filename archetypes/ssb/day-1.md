---
title: "{{ replace .Name "-" " " | title }} - Day 1"
date: {{ dateFormat "2006-01-02" .Date }}
draft: true

type: "posts"

summary: >-
  ""

images: "/images/{{ .Name }}.webp"
---
