---
title: "Chase Hospitals"
layout: splash
permalink: /chase-hospitals/
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/logo-2.jpg
  actions:
    - label: "View Source Code"
      url: "https://github.com/luciferchase/chase_hospitals"

intro: 
  - excerpt: "This is a GUI-based system which provide best solution for future's computerised interactions plus this Software uses offline Text to Speech software so that handicapped patients will have greater ease of access while running this software. All the data's are stored in tabular form in a relational database i.e. MySQL database with Tkinter based GUI written in Python."

feature_row_about:
  - image_path: assets/images/python-connectivity-mysql.webp
    alt: "About"
    title: "About the project"
    excerpt: "This is a GUI based Python connectivity project on Hospital Management. The front-end is made using Tkinter and the back-end is managed by MySQL. This project was made for our final year CBSE practicals by Udit Pati and Robin Vats"
    url: "/chase-hospitals/about/"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_features:
  - image_path: /assets/images/features.webp
    alt: "Features"
    title: "See Features"
    excerpt: "Talking about the features of this Hospital Management System, this project is aimed for a completely computerised management of our fictional hospital **Chase Hospitals**. A patient can register themselves, view their details and modify their details as well. They can see the Details of Doctors, view the Services offered by the hospital. They can also make an appointment to a particular doctor."
    url: "/chase-hospitals/features/"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_working:
  - image_path: /assets/images/inner-working.webp
    alt: "Working"
    title: "Working Description"
    excerpt: "This project took pretty long. I didn't knew much about Tkinter so it was pretty much hands-on learning only. Still pretty much satisfied with the end result. My problems and solutions as well as working description are discussed in details here."
    url: "/chase-hospitals/working/"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_installation:
  - image_path: /assets/images/download.webp
    alt: "Download"
    title: "Download Project"
    excerpt: "There are numerous ways to install and run this project in your local computer. The easiest is to just download its zip file and unzip. However if you know git clone this repo (and make sure to leave a star) and run in your local computer."
    url: "/chase-hospitals/installation/"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row_developers:
  - image_path: /assets/images/developers.webp
    alt: "Lucifer Chase"
    title: "Developers"
    excerpt: "This project is created by **Udit Pati** and **Robin Vats** as part of their 12th CS project 2020 - 2021, under the able and very helpful guidance of PGT Mr. ML Meena Sir, Kendriya Vidyalaya No. 2 Delhi Cantt."
    url: "/about/"
    btn_label: "Read More"
    btn_class: "btn--primary"

excerpt: "A GUI based Python Connectivity project on Hospital Management. The front-end is made using Tkinter while the back-end is managed by MySQL. Project created by Udit Pati and Robin Vats."
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="feature_row_about" type="left" %}

{% include feature_row id="feature_row_features" type="right" %}

{% include feature_row id="feature_row_working" type="left" %}

{% include feature_row id="feature_row_installation" type="right" %}

{% include feature_row id="feature_row_developers" type="left" %}