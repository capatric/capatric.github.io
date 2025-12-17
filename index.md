---
layout: default
title: Home
---

# Ensuring the Reliability of AI Infrastructure

I am an **Electronics Engineer** and **Site Reliability Engineer** at Oracle.
I specialize in Cloud Infrastructure, Linux systems, and Hardware Automation.

[More About Me &rarr;](/about)

### Recent Posts
<ul>
  {% for post in site.posts limit:3 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span style="color: #888; font-size: 0.9rem;">- {{ post.date | date: "%B %d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>
