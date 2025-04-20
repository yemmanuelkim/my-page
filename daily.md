---
layout: default
title: Daily
permalink: /daily/
---

<h1>Daily</h1>

<div class="post-grid">
  {% for post in site.posts %}
    {% if post.categories contains "daily" %}
      <div class="post-card">
        <h2<a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
        <p>{{ post.excerpt }}</p>
        <a class="read-more" href="{{ post.url }}">Read more →</a>
      </div>
    {% endif %}
  {% endfor %}
</div>
