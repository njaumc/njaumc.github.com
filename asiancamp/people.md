---
layout: asiancamp
title: "People"
description: ""
---
Asian Camp Design Team:

{% for person in site.data.ac_people %}
<div class="media">
  <a class="pull-left">
    <img class="media-object img-rounded profile-picture" src="{{person.image}}">
  </a>
  <div class="media-body">
    <h3 class="media-heading">{{person.name}}</h3>
    <div class="media">
      <ul>
        {% for desc in person.description %}
        <p>{{desc}}</p>
        {% endfor %}
        {{person.scripture}}
      </ul>
    </div>
  </div>
</div>
{% endfor %}

