---
title: Blog
layout: default
permalink: /blog/
show_tag_menu_link: true
---

{% if page.show_tag_menu_link %}
  <p class="blog-tag-link">
    <a href="{{ site.baseurl }}/tags/">Browse by tag</a>
  </p>
{% endif %}

<ul class="post-list">
{% for post in site.posts reversed %}
	<li>
	
		<h3 style="margin-bottom: 5px">
		<a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
		</h3>
		
		<span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
	</li>
{% endfor %}
</ul>

<!--<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>-->

