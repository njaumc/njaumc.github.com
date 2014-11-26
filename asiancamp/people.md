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
    <h3 class="media-heading">{{person.name}} <small>{{person.church}}</small></h3>
    <div class="media">
      <ul>
        <li>Quote: {{person.quote}}</li>
        <li>Scripture: {{person.scripture}} </li>
        <li>Occupation: {{person.occupation}} </li>
        <li>Years at Camp: {{person.years}} </li>
      </ul>
      <p>
        {{person.blurb}}
      </p>
    </div>
  </div>
</div>
{% endfor %}

