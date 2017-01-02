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
        {% if person.quote and person.quote1 %}
        <li>Quotes:</li>
        <ul>
          <li>{{person.quote}}</li>
          <li>{{person.quote1}}</li>
        </ul>
        {% else %}
        <li>Quote: {{person.quote}}</li>
        {% endif %}

        <li>Scripture: {{person.scripture}} </li>
        <li>Occupation: {{person.occupation}} </li>
        <li>Years at Camp: {{person.years}} </li>
        <li>Two animals you’d like to be best friends: {{person.animals}}</li>
      </ul>
      <p>
        {{person.why}}
      </p>
    </div>
  </div>
</div>
{% endfor %}

