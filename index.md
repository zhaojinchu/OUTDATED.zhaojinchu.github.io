---
layout: home
title: Home
---
{% assign dateStart = "2007-06-03" | date: '%s' %}
{% assign nowTimestamp = 'now' | date: '%s' %}
{% assign diffSeconds = nowTimestamp | minus: dateStart %}
{% assign diffDays = diffSeconds | divided_by: 3600 | divided_by: 24 | divided_by: 365 %}


# About

Hi all, I'm Zhaojin, a {{ diffDays | round: 0 }} year old student studying at Dubai College. I play tennis, listen to music, and practice music on my two instruments: piano and viola. For all other times, you can find me working on my projects and programming code. 

My interests include web dev, artificial intelligence, processor architectures, hardware simulations, and learning about completely new things once in a while. 

I do most of my programming in python, with proficiency in html, css, and VHDL. I also have experience with KiCad, schematics, and dabbled with PCB layouts and printing.


# Projects
{% include projects.html %}



# Curriculum Vitæ
[Click here](cv) to see my CV page, and [here](assets/files/cv.pdf) to download or view a pdf print version.

# Contact Me
{% include contact.html %}




<!--
Template has blog function - NOT IN USE
{% include archive.html %}
-->