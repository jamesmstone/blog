---
layout: page
title: "James' Blog"
---

## Welcome to James Stone's Personal Blog

This site is still heavily under development...

{% assign loopindex = 0 %}
{% for page in site.posts %}                       
   {% assign loopindex = loopindex | plus: 1 %}
   {% assign rowfinder = loopindex | modulo: 4 %}
   {% if rowfinder == 1 %}
   <div class="row">
   {% endif %}
   <div class="three columns">
      <h3>{{ page.title }}</h3>
   </div>
   {% if rowfinder == 0 %}
   </div>
   {% endif %}
{% endfor %}
{% if rowfinder != 0 %}
</div>
{% endif %}
    

