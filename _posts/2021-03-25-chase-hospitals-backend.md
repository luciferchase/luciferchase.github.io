---
title: "Backend"
last_modified_at: 2021-03-25
categories:
  - Chase Hospitals
tags:
  - Backend
  - Inner Working
  - Chase Hospital
  - Python - MySQL connectivity
---

# Connecting to Database

As soon as you enter the main window, you are asked to fill your MySQL username and password. 
By-default your username is taken as root, however you can change it. 

![mysql-username](/assets/Screenshots/mysql_username.jpg)

After this you are asked to write your password. The password is hidden with a string of asterisks. Pretty cool feature by EasyGUI.

![mysql-password](/assets/Screenshots/mysql_password.jpg)

You will see the style of the dialog box is slightly different. This is because I had used EasyGUI library here instead of Tkinter. At that time I knew about Tkinter and making a password-dialog box was above my skillset. EasyGUI is pretty good for these kind of things however it lacks customisation.
