---
{{ $name := substr .File.Dir 4 -1 }}
{{ $slice := split $name "-" }}
{{ $title := delimit (slice (index $slice 0 | upper) (index $slice 1 | title)) " " }}
title: {{ $title }} - Day 2
date: {{ dateFormat "2006-01-02" .Date }}
draft: true

type: "posts"

summary: >-

images: ["/images/{{ $name }}.webp"]
---
