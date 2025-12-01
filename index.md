---
layout: default
title: "My Mathematical Blog"
---

# Recent Posts

<ul class="post-list">
  {% for post in site.posts %}
    <li>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

      <h2>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h2>

      {{ post.excerpt }} 

      <p>
        <a href="{{ post.url | relative_url }}">Continue reading...</a>
      </p>
    </li>
  {% endfor %}
</ul>
