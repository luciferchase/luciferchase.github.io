---
weight: 0
{{ $name := substr .File.Dir 4 -1 }}
{{ $slice := split $name "-" }}
{{ $title := delimit (slice (index $slice 0 | upper) (index $slice 1 | title)) " " }}
title: {{ $title }}
date: {{ dateFormat "2006-01-02" .Date }}
draft: true
url: "/ssb/{{ $name }}/"

type: "posts"
hiddenFromHomePage: false

categories: ["ssb-stories"]
tags: ["SSB"]

summary: >-
  **Place**: -{{ $title }}
  **Date**:
  **Batch**:
  **Result**:

featuredImage: "/images/{{ $name }}.webp"
images: ["/images/{{ $name }}.webp"]
toc:
  enable: false
---

# tl;dr
**Place**:\
**Date**:\
**Batch**:\
**Result**:\

# Introduction

# My Experience in SSB

{{< admonition type=warning title="Work in Progress" >}}
[**Day 1**](/ssb/{{ $name }}/day-1): Screen-in\
[**Day 2**](/ssb/{{ $name }}/day-2): Psychology Tests\
[**Day 3**](/ssb/{{ $name }}/day-3): GTO day\
[**Day 4**](/ssb/{{ $name }}/day-4): Interview\
[**Day 5**](/ssb/{{ $name }}/day-5): Conference
{{< /admonition >}}
