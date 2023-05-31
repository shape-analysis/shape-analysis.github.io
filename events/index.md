---
layout: page
title: "Shape analysis"
description: "Events"
background: "../img/banner_5.png"
---


### Events, workshops and conferences

<hr>
{% for oneitem in site.data.events %}
   <h5>{{ oneitem.date }} &#8212; {{ oneitem.title }}</h5>
  <p>
  <b>Location:</b> {{ oneitem.location | markdownify | remove: '<p>' | remove: '</p>' }}
  <br/>
  <b>Web page:</b> <a href="{{ oneitem.url }}">link</a> <br/>
  <b>Abstract:</b> {{ oneitem.abstract | markdownify | remove: '<p>' | remove: '</p>'  }}
  </p>
  <hr>
{% endfor %}

