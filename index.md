---
layout: page
title: Home
tagline: LetsFiddle - Exploring the web
---
{% include JB/setup %}




  {% for post in site.posts %} 
  <div class="span8" >
     <h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2>
	{{post.excerpt}}
	<hr />
  </div>
  
<div class="span4" >
<span>{{ post.date | date_to_string }}</span> &raquo;
<br />
<img src="{{post.dpic}}" />
</div>
  {% endfor %}

