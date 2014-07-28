---
layout: page
title: Home
tagline: LetsFiddle - Exploring the web
---
{% include JB/setup %}




  {% for post in site.posts %} 
  
<div class="span4" style="float:left; min-height:200px;">
<span>{{ post.date | date_to_string }}</span> &raquo;
<br />
<img src="{{post.dpic}}" />
</div>

<div class="span8" style="float:right; min-height:200px;">
     <h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2>
	{{post.excerpt}}
	<hr />
  </div>

  {% endfor %}

