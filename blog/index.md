---
title: Blog
layout: default
permalink: /blog/
---

<ul class="post-list" style="margin-bottom: 5px; margin-bottom: 0px;">
{% for post in site.posts %}
	<li>
	
		<span class="post-meta"><font size="+2"><b>{{ post.date | date: "%b %-d, %Y" }}</b></font></span>

		<h2>
		<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
		</h2>
	</li>
{% endfor %}
</ul>

<!--<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>-->

