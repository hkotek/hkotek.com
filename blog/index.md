---
title: Blog
layout: default
permalink: /blog/
---

<ul class="post-list">
{% for post in site.posts %}
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
          <a class="tag" href="{{ site.baseurl }}/tags/{{ tag | slugify }}/">
            {{ tag }}
          </a>
        {% endfor %}
      </div>
    {% endif %}
  </li>
{% endfor %}
</ul>