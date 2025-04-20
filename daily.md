---
layout: default
title: Daily
permalink: /daily/
---

<h1>Daily</h1>

{% for post in site.posts %}
  {% if post.categories contains "daily" %}
    <div class="post-preview">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p>{{ post.excerpt }}</p>
    </div>
  {% endif %}
{% endfor %}
