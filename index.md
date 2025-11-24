---
layout: default
title: Home
---

# Hello, I'm Carlos Patricio

I'm a Electrinics Engineer focused on [your focus areas]. Currently working at Oracle as Site Reliability Engineer.

## What I Do

I specialize in working in the Artificial Intelligence Infrastructure team at Oraclre. My interests include Linux, new technologies, AI, Hardware Developement and so on.

## Recent Posts

{% for post in site.posts limit:3 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}

[View all posts →](/posts)

## Get in Touch

Feel free to reach out via [email](mailto:{{ site.email }}) or connect with me on [LinkedIn](https://linkedin.com/in/capatric).
