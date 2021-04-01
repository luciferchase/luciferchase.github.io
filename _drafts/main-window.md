---
title: "Main Window"
last_modified_at: 2021-03-27
categories:
  - blog
  - chase-hospitals
tags:
  - Frontend
  - Tkinter
  - Chase Hospitals
hide: true
---

In this post I will explain about the main window. Read how I created the color scheme, logo, design everythin for my main window.

# Structure

The window is fully maxim
The main window is divided into three parts:

- `top_frame`
- `left_frame`
- `right_frame`

If you don't know how this was done, [Read Here](/blog/chase-hospitals/design-and-structure/#frames){: .btn .btn--inverse}

## `top_frame`

The `top_frame` is constant throughout the whole application. The title `Chase Hospitals` is written here.

```python
# top frame (constant)
top_frame = LabelFrame(root)
top_frame.grid(row = 0, column = 0, rowspan = 2, columnspan = 8)
top_frame.grid_propagate(0)

# title
title = Label(top_frame, text = "Chase Hospitals", font = "evogria 45", 
			bg = "#FFE2E2", width = 42, anchor = CENTER)
title.pack()
```