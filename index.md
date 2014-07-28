---
layout: page
title: Home
tagline: LetsFiddle - Exploring the web
---
{% include JB/setup %}



<ul class="posts">
  {% for post in site.posts %} 
  
<div class="span4">
<span>{{ post.date | date_to_string }}</span> &raquo;
<br />
{{post.dpic}}
</div>

<div class="span8">
     <h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2>
	<br />{{post.excerpt | strip_html }}
  </div>
  <hr />
  {% endfor %}
</ul>
