---
layout: page
title: 首页
keywords: 技术,Java,码农
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
    <li>
		<span>{{ post.date | date_to_string }}</span> &raquo; 
		<a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
		<p>{{ post.content || split:'<!--break-->' | first | strip_html}}</p>
	</li>
  {% endfor %}
</ul>

