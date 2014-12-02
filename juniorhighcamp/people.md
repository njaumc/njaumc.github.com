---
layout: juniorhighcamp
title: "People"
description: ""
---
The directors of JHC are primary examples of leadership, servanthood, and devotion towards Christ.  Learn more about them below!

{% for person in site.data.jhc_people %}
<div class="media">
  <a class="pull-left">
    <img class="media-object img-rounded profile-picture" src="{{person.image}}">
  </a>
  <div class="media-body">
    <h3 class="media-heading">{{person.name}}</h3>
    <div class="media">
      {% if person.school %} <p>{{person.school}}</p> {% endif %}
      {% if person.occupation %} <p>{{person.occupation}}</p> {% endif %}
   		<p>{{person.blurb}}</p>
      {% if person.self %} <p>{{person.self}}</p> {% endif %}
      <p>Contact: <a href="mailto:{{person.email}}">{{person.email}}</a></p>
    </div>
  </div>
</div>
{% endfor %}

