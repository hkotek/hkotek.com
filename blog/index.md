---
title: Blog
layout: default
permalink: /blog/
show_tag_menu_link: true
---

<h1 class="blog-title">Posts</h1>

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
  </li>
{% endfor %}
</ul>

{% if page.show_tag_menu_link %}
  <div class="blog-tags-section">
    <h2>Browse by tag</h2>
    <ul class="tag-list">
      {% assign sorted_tags = site.tags | sort %}
      {% for tag in sorted_tags %}
        <li>
          <a href="{{ site.baseurl }}/tags/{{ tag[0] | slugify }}/">
            {{ tag[0] }} ({{ tag[1].size }})
          </a>
        </li>
      {% endfor %}
    </ul>
  </div>
{% endif %}

