---
layout: default
title: Home
description: Carlos Patricio builds reliable AI infrastructure and Linux automation for cloud and hardware-heavy environments.
---

# Ensuring the Reliability of AI Infrastructure

I am an **Electronics Engineer** and **Site Reliability Engineer** at Oracle.  
I specialize in cloud infrastructure, Linux systems, and hardware automation.

[More About Me &rarr;]({{ '/about' | relative_url }})

### Recent Posts

<ul>
  {% for post in site.posts limit:3 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span class="home-post-date">- {{ post.date | date: "%B %d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>
