---
layout: default
title: "Egor Malitskiy"
---

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <span class="post-meta">{{ post.date | date: "%B %d, %Y" }}</span>

      <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
      </a>

      <div class="post-excerpt">
        {{ post.excerpt }}
      </div>

      <a href="{{ post.url | relative_url }}" class="read-more">Full Story</a>
    </li>
  {% endfor %}
</ul>