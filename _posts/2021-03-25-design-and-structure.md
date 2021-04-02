---
title: "Design and Structure"
last_modified_at: 2021-03-26
categories:
  - blog
  - chase-hospitals
tags:
  - Tkinter
  - Chase Hospitals
feature_post: true
---

Read my initial problems and subsequent ideas to tackle those problems. A detailed description of the basic structure of main file is given here.

## Initial Brainstorm

We were required to make a python project which solves a real world problem. It must connect to a MySQL database and maintain some kind of record.

### Inspiration

To get some inspiration I found this pretty cool website which hosts large number of projects.
[Python Projects](http://python.mykvs.in/uploads/showpapers/testproject.php)

There were so many cool ideas regarding all kinds of things. I downloaded bunch of projects and ran it in my local computer. Two particular project caught my eye.

- [Banking System](http://python.mykvs.in/uploads/projects/XIComp.Sc.12.zip)

![idea-bank](/assets/Screenshots/idea_bank.jpg)

This project was simply brilliant. I was completely surprised that you can do these kinds of things with python too. I was stoked. The use of Tkinter, stylized fonts, idea, everything was amazing. I decided at that time to make a project using Tkinter only. This project also gave the idea for Text - to - Speech.

- [Hospital Management](http://python.mykvs.in/uploads/projects/XIIComp.Sc.47.zip)

![idea-hospital](/assets/Screenshots/idea_hospital.jpg)

This project was completely based on Tkinter. This project actually gave me the idea for Hospital Management. Seeing this I decided to make my project completely using Tkinter only

#### Initial Idea

After deciding our theme, both of us one day met on Skype (covid times :pensive:). I opened Whiteboard and quickly drew out whatever came to my mind. In retrospection this part was extremely important as it gave us a clear path to implement.

![initial-idea](/assets/Screenshots/brainstorm.jpg)    

In our design we would have 3 partitions in our main window. In the top part (`top_frame`) **Chase Hospitals** was to be written. In the left side (`left_frame`) all our buttons would be there. And at last in the right side (`right_frame`) the magic would happen. Initially our logo would be shown, but once you click on any button, this `right_frame` would change while the rest would remain exactly same.
This was our hack to make a responsive sidebar. Yes, it is very crude but hey, as long it works, it works :wink:.

After deciding this we quickly jot down ideas for buttons and what they would implement. Initially there was to be an Admin block too however due to shortage of time and other commitments we were not able to implement that and scraped that idea.

## Basic Structure

The main file is divided into three parts. 

- **Modules for Buttons** - Functions for all the button
- **`main_window()`** - This paints the main window
- **Backend** - All the backend functions after connecting with database

### Frames

After banging my head on the wall repeatedly and spending hours on the internet, still I was not able to implement how to make three separate partitions in the main window. Then I found out about `frames()`.

How `frames()` works is that it makes a separate window like partition inside a window. It acts completely independent of other content in the window.

```python
# top frame (constant)
top_frame = LabelFrame(root)
top_frame.grid(row = 0, column = 0, rowspan = 2, columnspan = 8)
top_frame.grid_propagate(0)
```

This creates a frame on the top of the window. Similarly other frames are also created.
Now instead of initializing the buttons and other stuff in the root window, I would initialize them on their designated frame.

In this way, the problem of different partition of the main window was solved. :tada: