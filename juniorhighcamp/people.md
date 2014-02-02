---
layout: juniorhighcamp
title: "People"
description: ""
---
The directors of JHC are primary examples of leadership, servanthood, and devotion towards Christ.  Learn more about them below!

{% for person in site.data.people %}
<div class="media">
  <a class="pull-left">
    <img class="media-object img-rounded profile-picture" src="{{person.image}}">
  </a>
  <div class="media-body">
    <h3 class="media-heading">{{person.name}} <small>{{person.church}}</small></h3>
    <div class="media">
    	<ul>
        <li>Quote: {{person.quote}}</li>
  			<li>Hobbies and Interests: {{person.hobbies}} </li>
		  </ul>
   		<p>
        {{person.blurb}}
  		</p>
    </div>
  </div>
</div>
{% endfor %}

