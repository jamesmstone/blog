---
layout: page
title: "James' Blog"
---

## Welcome to James Stone's Personal Blog

This site is still heavily under development...

{% for post in site.posts %}
    
####[{{ post.title }}]({{ post.url }})
{{ post.date | date_to_long_string }}
{% endfor %}
