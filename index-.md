---
layout: page
title: Home
tagline: LetsFiddle - Exploring the web
---
{% include JB/setup %}



<table><tr>
  {% for post in site.posts %} 
  <div class="span8" >
<span>{{ post.date | date_to_string }}</span> &raquo;
     <h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2>
	{{post.excerpt}}
	<hr />
  </div>
  
<div class="span3" style="float:right;" >
<img src="{{post.dpic}}" width="200px" />
</div>
  {% endfor %}
 </tr> </table>

