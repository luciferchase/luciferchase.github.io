---
{{ $name := substr .File.Dir 4 -1 }}
{{ $slice := split $name "-" }}
{{ $title := delimit (slice (index $slice 0 | upper) (index $slice 1 | title)) " " }}
title: "-{{ $title }} by Lucifer Chase"
url: "/ssb/{{ $name }}/all-days/"
---
