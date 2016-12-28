---
layout: asiancamp
title: "People"
description: ""
---
Asian Camp Design Team:

{% for person in site.data.ac_people %}
<h3>{{person.name}}</h3>
<div>
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
{% endfor %}

