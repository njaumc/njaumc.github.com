---
layout: asiancamp
title: "People"
description: ""
---
Asian Camp Design Team:

{% for person in site.data.ac_people %}
###{{person.name}} <small>{{person.church}}</small>

{% endfor %}