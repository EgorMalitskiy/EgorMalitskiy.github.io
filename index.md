---
layout: default
title: "Egor Malitskiy | Home"
---

<div class="intro-section">
  <h1>Welcome.</h1>
  <p>
    Hi, I'm <strong>Egor Malitskiy</strong>. I write about mathematics, physics, and the beautiful equations that describe our universe. 
    This is my digital garden where I share notes, derivations, and thoughts on my research.
  </p>
</div>

<h2>Recent Notes</h2>

<ul class="post-list">
  {% for post in site.posts %}
    <li class="post-item">
      <span class="post-meta">{{ post.date | date: "%B %-d, %Y" }}</span>

      <a class="post-link" href="{{ post.url | relative_url }}">
        {{ post.title }}
      </a>

      <div class="post-excerpt">
        {{ post.excerpt | strip_html | truncatewords: 30 }}
      </div>
      
      <a href="{{ post.url | relative_url }}" style="font-size: 0.9rem; font-weight: bold;">Read more &rarr;</a>
    </li>
  {% endfor %}
</ul>