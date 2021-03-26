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
  - excerpt: "This is a GUI-based system which provide best solution for future's computerised intractions plus this Software uses offline Text to Speech software so that handicapped patients will have greater ease of access while running this software. All the data's are stored in tabular form in a relational database i.e. MySQL database with tkinter based GUI written in Python."
feature_row_about:
  - image_path: assets/images/python-connectivity-mysql.jpg
    alt: "About"
    title: "About the project"
    excerpt: "Read what this project is all about."
    url: "/about/"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row_features:
  - image_path: /assets/images/features.jpg
    alt: "Features"
    title: "See Features"
    excerpt: "See features of this project with plenty of screenshots."
    url: "/features/"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row_working:
  - image_path: /assets/images/inner-working.jpg
    alt: "Working"
    title: "Working Description"
    excerpt: 'Read in detail, how I made this project. See the problems that I faced and their subsequent solutions.'
    url: "/working/"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row_installation:
  - image_path: /assets/images/download.jpg
    alt: "Download"
    title: "Download Project"
    excerpt: "Download this project and run it in your local computer."
    url: "/installation/"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row_developers:
  - image_path: /assets/images/developers.jpg
    alt: "Lucifer Chase"
    title: "Developers"
    excerpt: "Hola, that's me :wink:"
    url: "/installation/"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row id="feature_row_about" type="left" %}

{% include feature_row id="feature_row_features" type="right" %}

{% include feature_row id="feature_row_working" type="left" %}

{% include feature_row id="feature_row_installation" type="right" %}

{% include feature_row id="feature_row_developers" type="left" %}