---
layout: page
title: Home
tagline: LetsFiddle - Exploring the web
---
{% include JB/setup %}



<table><tr>
  {% for post in site.posts %} 
  <td>
  <div class="span8" >
     <h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h2>
	{{post.excerpt}}
	<hr />
  </div></td>
  <td>
<div class="span4" style="float:right;" >
<span>{{ post.date | date_to_string }}</span> &raquo;
<br />
<img src="{{post.dpic}}" />
</div> </td>
  {% endfor %}
</tr> </table>

