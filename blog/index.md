---
title: Blog
layout: default
permalink: /blog/
show_tag_menu_link: true
---

<div class="blog-header">
  <h1 class="blog-title">Posts</h1>

  {% if page.show_tag_menu_link %}
    <a class="blog-tag-link" href="{{ site.baseurl }}/tags/">
      Browse by tag
    </a>
  {% endif %}
</div>

<ul class="post-list">
{% for post in site.posts reversed %}
  <li>
    <h3 style="margin-bottom: 5px">
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">
        {{ post.title }}
      </a>
    </h3>

    <span class="post-meta">
      {{ post.date | date: "%b %-d, %Y" }}
    </span>

    {% if post.tags %}
      <div class="post-tags">
        {% for tag in post.tags %}
          <a href="{{ site.baseurl }}/tags/{{ tag | slugify }}/" class="tag">
            {{ tag }}
          </a>
        {% endfor %}
      </div>
    {% endif %}
  </li>
{% endfor %}
</ul>

<!--<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>-->

