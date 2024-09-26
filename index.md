---
layout: default
title: Home
---

## Blog Posts

{% for post in site.posts %}
  - [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

# Welcome to My Website
This is the homepage of my new Jekyll website
