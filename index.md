---
layout: page
title: Home
tagline: Exploring the web
---
{% include JB/setup %}



<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2></li>
  {% endfor %}
</ul>