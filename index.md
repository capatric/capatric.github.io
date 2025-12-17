---
layout: default
title: Home
---

<!-- 1. The Hero Section: Big and bold -->
# Building the Infrastructure Behind AI.

I am an **Electronics Engineer** and **Site Reliability Engineer** at Oracle.  
I specialize in Cloud Infrastructure, Linux systems, and Hardware Automation.

<br>

<!-- 2. Call to Action: Direct them to your Resume/About page -->
[More About Me →](/about)

---

<!-- 3. Recent Posts (Optional: Only keep if you write blogs) -->
### Recent Posts
<ul>
  {% for post in site.posts limit:3 %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span style="color: #888; font-size: 0.9rem;">- {{ post.date | date: "%B %d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>
