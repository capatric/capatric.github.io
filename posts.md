---
layout: page
title: Posts
description: Writing archive for Carlos Patricio on reliability, automation, and validation.
eyebrow: Writing
intro: Notes on infrastructure reliability, hardware-aware debugging, and the engineering habits that keep systems maintainable.
---

<div class="post-list">
{% for post in site.posts %}
  <article class="post-card">
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }}</p>
    <a class="text-link" href="{{ post.url }}">Read post</a>
  </article>
{% endfor %}
</div>
