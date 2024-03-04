---
layout: page
title: Avisos
nav_exclude: false
description: A feed containing all of the class announcements.
---

# Avisos

Lista completa de avisos desde o começo da disciplina:

{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}
