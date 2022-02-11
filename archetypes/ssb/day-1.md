---
{{ $name := substr .File.Dir 4 -1 }}
{{ $slice := split $name "-" }}
{{ $title := delimit (slice (index $slice 0 | upper) (index $slice 1 | title)) " " }}
title: -{{ $title }} - Day 1
date: {{ dateFormat "2006-01-02" .Date }}
draft: true

type: "posts"
hiddenFromHomePage: false

summary: >-

images: ["/images/{{ $name }}.webp"]
---

{{< image src="/images/{{ $name }}.webp" caption="Me and my bois (I am Chest No. )" height=100% width=100% >}}

This blog owing to its length is divided into 5 posts, each in detail description of my 5 day experience in the SSB. After reading this checkout the rest of the Posts too [All -{{ $title }} by Me](/ssb/{{ $name }}/all-days).\
Read summary of this SSB [-{{ $title }}](/ssb/{{ $name }}).\
Read all my SSB attempts: [SSB Stories](/categories/ssb-stories).

Checkout - [Day 2](/ssb/{{ $name }}/day-2/)\
[All my days at 1-AFSB Dehradun](/ssb/{{ $name }}/all-days/)

Peace.
