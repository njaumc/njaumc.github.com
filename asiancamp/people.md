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
    <li>Quote: {{person.quote}}</li>
    <li>Scripture: {{person.scripture}} </li>
    {% if person.occupation %}<li>Occupation: {{person.occupation}} </li>{% endif %}
    {% if person.years %}<li>Years at Camp: {{person.years}} </li>{% endif %}
    <li>Two animals you’d like to be best friends: {{person.animals}}</li>
  </ul>
  <p>
    {{person.why}}
  </p>
</div>
{% endfor %}

